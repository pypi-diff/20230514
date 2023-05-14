# Comparing `tmp/vnpy_tap-9.3.8.tar.gz` & `tmp/vnpy_tap-9.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_tap-9.3.8.tar", last modified: Sun Apr 23 04:25:42 2023, max compression
+gzip compressed data, was "vnpy_tap-9.3.9.tar", last modified: Fri May 12 00:36:46 2023, max compression
```

## Comparing `vnpy_tap-9.3.8.tar` & `vnpy_tap-9.3.9.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.849172 vnpy_tap-9.3.8/
--rw-rw-rw-   0        0        0     1109 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/LICENSE
--rw-rw-rw-   0        0        0       61 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2676 2023-04-23 04:25:42.850177 vnpy_tap-9.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1668 2023-04-23 04:25:25.000000 vnpy_tap-9.3.8/README.md
--rw-rw-rw-   0        0        0     1125 2023-04-23 04:25:42.852179 vnpy_tap-9.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2121 2023-04-17 12:55:32.000000 vnpy_tap-9.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.539608 vnpy_tap-9.3.8/vnpy_tap/
--rw-rw-rw-   0        0        0     1351 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.624743 vnpy_tap-9.3.8/vnpy_tap/api/
--rw-rw-rw-   0        0        0   144384 2022-05-11 03:09:57.000000 vnpy_tap-9.3.8/vnpy_tap/api/TapDataCollectAPI.dll
--rw-rw-rw-   0        0        0   524288 2020-09-26 07:16:56.000000 vnpy_tap-9.3.8/vnpy_tap/api/TapQuoteAPI.dll
--rw-rw-rw-   0        0        0       83 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.693008 vnpy_tap-9.3.8/vnpy_tap/api/generator/
--rw-rw-rw-   0        0        0      211 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_header_define.h
--rw-rw-rw-   0        0        0      103 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_header_function.h
--rw-rw-rw-   0        0        0      592 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_header_on.h
--rw-rw-rw-   0        0        0      331 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_header_process.h
--rw-rw-rw-   0        0        0      485 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_function.cpp
--rw-rw-rw-   0        0        0      481 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_module.cpp
--rw-rw-rw-   0        0        0     1886 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_on.cpp
--rw-rw-rw-   0        0        0     8834 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_process.cpp
--rw-rw-rw-   0        0        0      606 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_switch.cpp
--rw-rw-rw-   0        0        0     2629 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_task.cpp
--rw-rw-rw-   0        0        0     1507 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_header_define.h
--rw-rw-rw-   0        0        0     1288 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_header_function.h
--rw-rw-rw-   0        0        0     4184 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_header_on.h
--rw-rw-rw-   0        0        0     2217 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_header_process.h
--rw-rw-rw-   0        0        0     8476 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_function.cpp
--rw-rw-rw-   0        0        0     3743 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_module.cpp
--rw-rw-rw-   0        0        0    12515 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_on.cpp
--rw-rw-rw-   0        0        0    69618 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_process.cpp
--rw-rw-rw-   0        0        0     4084 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_switch.cpp
--rw-rw-rw-   0        0        0    18416 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_task.cpp
--rw-rw-rw-   0        0        0  4065280 2023-01-17 09:39:27.000000 vnpy_tap-9.3.8/vnpy_tap/api/iTapTradeAPI_64.dll
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.519784 vnpy_tap-9.3.8/vnpy_tap/api/include/
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.750762 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/
--rw-rw-rw-   0        0        0    19435 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     4434 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    88397 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     6778 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      122 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2030 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.773822 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/
--rw-rw-rw-   0        0        0    25522 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    38263 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     7905 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    16680 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    13759 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0     1482 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/typeid.h
--rw-rw-rw-   0        0        0    29541 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0     7611 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     3982 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     3039 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     5593 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    67353 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0     8917 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2096 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/options.h
--rw-rw-rw-   0        0        0    90857 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0    52650 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/pytypes.h
--rw-rw-rw-   0        0        0    13988 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    22206 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/stl_bind.h
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.800738 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/
--rw-rw-rw-   0        0        0     7211 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/TapAPICommDef.h
--rw-rw-rw-   0        0        0    20316 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/TapAPIError.h
--rw-rw-rw-   0        0        0    11989 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/TapQuoteAPI.h
--rw-rw-rw-   0        0        0     6198 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/TapQuoteAPIDataType.h
--rw-rw-rw-   0        0        0    10601 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/iTapAPICommDef.h
--rw-rw-rw-   0        0        0    28638 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/iTapAPIError.h
--rw-rw-rw-   0        0        0    64218 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/iTapTradeAPI.h
--rw-rw-rw-   0        0        0   112421 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/include/tap/iTapTradeAPIDataType.h
--rw-rw-rw-   0        0        0   152170 2023-01-17 09:28:36.000000 vnpy_tap-9.3.8/vnpy_tap/api/libTapDataCollectAPI.so
--rw-rw-rw-   0        0        0   352070 2020-09-26 08:34:14.000000 vnpy_tap-9.3.8/vnpy_tap/api/libTapQuoteAPI.so
--rw-rw-rw-   0        0        0   932084 2023-01-17 09:28:36.000000 vnpy_tap-9.3.8/vnpy_tap/api/libiTapTradeAPI.so
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.807551 vnpy_tap-9.3.8/vnpy_tap/api/libs/
--rw-rw-rw-   0        0        0     2712 2020-09-26 07:16:52.000000 vnpy_tap-9.3.8/vnpy_tap/api/libs/TapQuoteAPI.lib
--rw-rw-rw-   0        0        0     2620 2023-01-17 09:39:26.000000 vnpy_tap-9.3.8/vnpy_tap/api/libs/iTapTradeAPI_64.lib
--rw-rw-rw-   0        0        0    23745 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/tap_constant.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.810568 vnpy_tap-9.3.8/vnpy_tap/api/vntap/
--rw-rw-rw-   0        0        0     3765 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntap.h
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.824622 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/
--rw-rw-rw-   0        0        0      448 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/dllmain.cpp
--rw-rw-rw-   0        0        0       21 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/stdafx.cpp
--rw-rw-rw-   0        0        0      374 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/stdafx.h
--rw-rw-rw-   0        0        0      296 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/targetver.h
--rw-rw-rw-   0        0        0    23969 2023-04-17 12:43:06.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/vntapmd.cpp
--rw-rw-rw-   0        0        0     6895 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/vntapmd.h
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.840701 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/
--rw-rw-rw-   0        0        0      448 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/dllmain.cpp
--rw-rw-rw-   0        0        0       21 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/stdafx.cpp
--rw-rw-rw-   0        0        0      374 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/stdafx.h
--rw-rw-rw-   0        0        0      296 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/targetver.h
--rw-rw-rw-   0        0        0   136530 2023-04-17 12:56:18.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/vntaptd.cpp
--rw-rw-rw-   0        0        0    37333 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/vntaptd.h
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.846699 vnpy_tap-9.3.8/vnpy_tap/gateway/
--rw-rw-rw-   0        0        0       37 2023-04-17 12:24:10.000000 vnpy_tap-9.3.8/vnpy_tap/gateway/__init__.py
--rw-rw-rw-   0        0        0    25529 2023-04-23 04:24:54.000000 vnpy_tap-9.3.8/vnpy_tap/gateway/tap_gateway.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:25:42.572851 vnpy_tap-9.3.8/vnpy_tap.egg-info/
--rw-rw-rw-   0        0        0     2676 2023-04-23 04:25:42.000000 vnpy_tap-9.3.8/vnpy_tap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3462 2023-04-23 04:25:42.000000 vnpy_tap-9.3.8/vnpy_tap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 04:25:42.000000 vnpy_tap-9.3.8/vnpy_tap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-23 04:25:42.000000 vnpy_tap-9.3.8/vnpy_tap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-04-23 04:25:42.000000 vnpy_tap-9.3.8/vnpy_tap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 04:25:42.000000 vnpy_tap-9.3.8/vnpy_tap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.571724 vnpy_tap-9.3.9/
+-rw-rw-rw-   0        0        0     1109 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/LICENSE
+-rw-rw-rw-   0        0        0       61 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2676 2023-05-12 00:36:46.571724 vnpy_tap-9.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1668 2023-05-12 00:35:53.000000 vnpy_tap-9.3.9/README.md
+-rw-rw-rw-   0        0        0     1125 2023-05-12 00:36:46.574728 vnpy_tap-9.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2121 2023-04-17 12:55:32.000000 vnpy_tap-9.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:45.229714 vnpy_tap-9.3.9/vnpy_tap/
+-rw-rw-rw-   0        0        0     1351 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:45.655884 vnpy_tap-9.3.9/vnpy_tap/api/
+-rw-rw-rw-   0        0        0   144384 2022-05-11 03:09:57.000000 vnpy_tap-9.3.9/vnpy_tap/api/TapDataCollectAPI.dll
+-rw-rw-rw-   0        0        0   524288 2020-09-26 07:16:56.000000 vnpy_tap-9.3.9/vnpy_tap/api/TapQuoteAPI.dll
+-rw-rw-rw-   0        0        0       83 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:45.968288 vnpy_tap-9.3.9/vnpy_tap/api/generator/
+-rw-rw-rw-   0        0        0      211 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_header_define.h
+-rw-rw-rw-   0        0        0      103 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_header_function.h
+-rw-rw-rw-   0        0        0      592 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_header_on.h
+-rw-rw-rw-   0        0        0      331 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_header_process.h
+-rw-rw-rw-   0        0        0      485 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_function.cpp
+-rw-rw-rw-   0        0        0      481 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_module.cpp
+-rw-rw-rw-   0        0        0     1886 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_on.cpp
+-rw-rw-rw-   0        0        0     8834 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_process.cpp
+-rw-rw-rw-   0        0        0      606 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_switch.cpp
+-rw-rw-rw-   0        0        0     2629 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_task.cpp
+-rw-rw-rw-   0        0        0     1507 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_header_define.h
+-rw-rw-rw-   0        0        0     1288 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_header_function.h
+-rw-rw-rw-   0        0        0     4184 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_header_on.h
+-rw-rw-rw-   0        0        0     2217 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_header_process.h
+-rw-rw-rw-   0        0        0     8476 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_function.cpp
+-rw-rw-rw-   0        0        0     3743 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_module.cpp
+-rw-rw-rw-   0        0        0    12515 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_on.cpp
+-rw-rw-rw-   0        0        0    69618 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_process.cpp
+-rw-rw-rw-   0        0        0     4084 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_switch.cpp
+-rw-rw-rw-   0        0        0    18416 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_task.cpp
+-rw-rw-rw-   0        0        0  4065280 2023-01-17 09:39:27.000000 vnpy_tap-9.3.9/vnpy_tap/api/iTapTradeAPI_64.dll
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:45.196729 vnpy_tap-9.3.9/vnpy_tap/api/include/
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.201934 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/
+-rw-rw-rw-   0        0        0    19435 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     4434 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    88397 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     6778 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      122 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2030 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.285605 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    25522 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    38263 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     7905 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    16680 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    13759 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0     1482 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/typeid.h
+-rw-rw-rw-   0        0        0    29541 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0     7611 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     3982 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     3039 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     5593 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    67353 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0     8917 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2096 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/options.h
+-rw-rw-rw-   0        0        0    90857 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0    52650 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/pytypes.h
+-rw-rw-rw-   0        0        0    13988 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    22206 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/stl_bind.h
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.422148 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/
+-rw-rw-rw-   0        0        0     7211 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/TapAPICommDef.h
+-rw-rw-rw-   0        0        0    20316 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/TapAPIError.h
+-rw-rw-rw-   0        0        0    11989 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/TapQuoteAPI.h
+-rw-rw-rw-   0        0        0     6198 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/TapQuoteAPIDataType.h
+-rw-rw-rw-   0        0        0    10601 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/iTapAPICommDef.h
+-rw-rw-rw-   0        0        0    28638 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/iTapAPIError.h
+-rw-rw-rw-   0        0        0    64218 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/iTapTradeAPI.h
+-rw-rw-rw-   0        0        0   112421 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/include/tap/iTapTradeAPIDataType.h
+-rw-rw-rw-   0        0        0   152170 2023-01-17 09:28:36.000000 vnpy_tap-9.3.9/vnpy_tap/api/libTapDataCollectAPI.so
+-rw-rw-rw-   0        0        0   352070 2020-09-26 08:34:14.000000 vnpy_tap-9.3.9/vnpy_tap/api/libTapQuoteAPI.so
+-rw-rw-rw-   0        0        0   932084 2023-01-17 09:28:36.000000 vnpy_tap-9.3.9/vnpy_tap/api/libiTapTradeAPI.so
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.444148 vnpy_tap-9.3.9/vnpy_tap/api/libs/
+-rw-rw-rw-   0        0        0     2712 2020-09-26 07:16:52.000000 vnpy_tap-9.3.9/vnpy_tap/api/libs/TapQuoteAPI.lib
+-rw-rw-rw-   0        0        0     2620 2023-01-17 09:39:26.000000 vnpy_tap-9.3.9/vnpy_tap/api/libs/iTapTradeAPI_64.lib
+-rw-rw-rw-   0        0        0    23745 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/tap_constant.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.455146 vnpy_tap-9.3.9/vnpy_tap/api/vntap/
+-rw-rw-rw-   0        0        0     3765 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntap.h
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.514716 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/
+-rw-rw-rw-   0        0        0      448 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/dllmain.cpp
+-rw-rw-rw-   0        0        0       21 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/stdafx.cpp
+-rw-rw-rw-   0        0        0      374 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/stdafx.h
+-rw-rw-rw-   0        0        0      296 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/targetver.h
+-rw-rw-rw-   0        0        0    23969 2023-04-17 12:43:06.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/vntapmd.cpp
+-rw-rw-rw-   0        0        0     6895 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/vntapmd.h
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.551708 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/
+-rw-rw-rw-   0        0        0      448 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/dllmain.cpp
+-rw-rw-rw-   0        0        0       21 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/stdafx.cpp
+-rw-rw-rw-   0        0        0      374 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/stdafx.h
+-rw-rw-rw-   0        0        0      296 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/targetver.h
+-rw-rw-rw-   0        0        0   136530 2023-04-17 12:56:18.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/vntaptd.cpp
+-rw-rw-rw-   0        0        0    37333 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/vntaptd.h
+-rw-rw-rw-   0        0        0   705024 2023-04-23 04:26:03.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntapmd.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0   947200 2023-04-23 04:25:57.000000 vnpy_tap-9.3.9/vnpy_tap/api/vntaptd.cp310-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:46.567720 vnpy_tap-9.3.9/vnpy_tap/gateway/
+-rw-rw-rw-   0        0        0       37 2023-04-17 12:24:10.000000 vnpy_tap-9.3.9/vnpy_tap/gateway/__init__.py
+-rw-rw-rw-   0        0        0    24778 2023-05-12 00:30:05.000000 vnpy_tap-9.3.9/vnpy_tap/gateway/tap_gateway.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:36:45.275724 vnpy_tap-9.3.9/vnpy_tap.egg-info/
+-rw-rw-rw-   0        0        0     2676 2023-05-12 00:36:44.000000 vnpy_tap-9.3.9/vnpy_tap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3544 2023-05-12 00:36:45.000000 vnpy_tap-9.3.9/vnpy_tap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 00:36:44.000000 vnpy_tap-9.3.9/vnpy_tap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-12 00:36:44.000000 vnpy_tap-9.3.9/vnpy_tap.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-05-12 00:36:44.000000 vnpy_tap-9.3.9/vnpy_tap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 00:36:44.000000 vnpy_tap-9.3.9/vnpy_tap.egg-info/top_level.txt
```

### Comparing `vnpy_tap-9.3.8/LICENSE` & `vnpy_tap-9.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/PKG-INFO` & `vnpy_tap-9.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_tap
-Version: 9.3.8
+Version: 9.3.9
 Summary: TAP gateway for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 # VeighNa框架的易盛外盘交易接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-9.3.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-9.3.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_tap-9.3.8/README.md` & `vnpy_tap-9.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的易盛外盘交易接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-9.3.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-9.3.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_tap-9.3.8/setup.cfg` & `vnpy_tap-9.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7461 700d 0a76 6572   = vnpy_tap..ver
-00000020: 7369 6f6e 203d 2039 2e33 2e38 0d0a 7572  sion = 9.3.8..ur
+00000020: 7369 6f6e 203d 2039 2e33 2e39 0d0a 7572  sion = 9.3.9..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 7777 772e  l = https://www.
 00000040: 766e 7079 2e63 6f6d 0d0a 6c69 6365 6e73  vnpy.com..licens
 00000050: 6520 3d20 4d49 540d 0a61 7574 686f 7220  e = MIT..author 
 00000060: 3d20 5869 616f 796f 7520 4368 656e 0d0a  = Xiaoyou Chen..
 00000070: 6175 7468 6f72 5f65 6d61 696c 203d 2078  author_email = x
 00000080: 6961 6f79 6f75 2e63 6865 6e40 6d61 696c  iaoyou.chen@mail
 00000090: 2e76 6e70 792e 636f 6d0d 0a64 6573 6372  .vnpy.com..descr
```

### Comparing `vnpy_tap-9.3.8/setup.py` & `vnpy_tap-9.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/__init__.py` & `vnpy_tap-9.3.9/vnpy_tap/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/TapDataCollectAPI.dll` & `vnpy_tap-9.3.9/vnpy_tap/api/TapDataCollectAPI.dll`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/TapQuoteAPI.dll` & `vnpy_tap-9.3.9/vnpy_tap/api/TapQuoteAPI.dll`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_header_on.h` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_header_on.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_on.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_on.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_process.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_process.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_switch.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_switch.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_md_source_task.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_md_source_task.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_header_define.h` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_header_define.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_header_function.h` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_header_function.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_header_on.h` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_header_on.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_header_process.h` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_header_process.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_function.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_function.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_module.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_module.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_on.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_on.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_process.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_process.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_switch.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_switch.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/generator/tap_td_source_task.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/generator/tap_td_source_task.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/iTapTradeAPI_64.dll` & `vnpy_tap-9.3.9/vnpy_tap/api/iTapTradeAPI_64.dll`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/attr.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/buffer_info.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/cast.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/chrono.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/complex.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/class.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/common.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/descr.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/init.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/internals.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/detail/typeid.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/eigen.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/embed.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/eval.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/functional.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/iostream.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/numpy.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/operators.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/options.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/pybind11.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/pytypes.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/stl.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/pybind11/stl_bind.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/tap/TapAPICommDef.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/tap/TapAPICommDef.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/tap/TapAPIError.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/tap/TapAPIError.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/tap/TapQuoteAPI.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/tap/TapQuoteAPI.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/tap/TapQuoteAPIDataType.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/tap/TapQuoteAPIDataType.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/tap/iTapAPICommDef.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/tap/iTapAPICommDef.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/tap/iTapAPIError.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/tap/iTapAPIError.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/tap/iTapTradeAPI.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/tap/iTapTradeAPI.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/include/tap/iTapTradeAPIDataType.h` & `vnpy_tap-9.3.9/vnpy_tap/api/include/tap/iTapTradeAPIDataType.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/libTapDataCollectAPI.so` & `vnpy_tap-9.3.9/vnpy_tap/api/libTapDataCollectAPI.so`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/libTapQuoteAPI.so` & `vnpy_tap-9.3.9/vnpy_tap/api/libTapQuoteAPI.so`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/libiTapTradeAPI.so` & `vnpy_tap-9.3.9/vnpy_tap/api/libiTapTradeAPI.so`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/libs/TapQuoteAPI.lib` & `vnpy_tap-9.3.9/vnpy_tap/api/libs/TapQuoteAPI.lib`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/libs/iTapTradeAPI_64.lib` & `vnpy_tap-9.3.9/vnpy_tap/api/libs/iTapTradeAPI_64.lib`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/tap_constant.py` & `vnpy_tap-9.3.9/vnpy_tap/api/tap_constant.py`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntap.h` & `vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntap.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/vntapmd.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/vntapmd.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntapmd/vntapmd.h` & `vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntapmd/vntapmd.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/vntaptd.cpp` & `vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/vntaptd.cpp`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap/api/vntap/vntaptd/vntaptd.h` & `vnpy_tap-9.3.9/vnpy_tap/api/vntap/vntaptd/vntaptd.h`

 * *Files identical despite different names*

### Comparing `vnpy_tap-9.3.8/vnpy_tap.egg-info/PKG-INFO` & `vnpy_tap-9.3.9/vnpy_tap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-tap
-Version: 9.3.8
+Version: 9.3.9
 Summary: TAP gateway for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 # VeighNa框架的易盛外盘交易接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-9.3.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-9.3.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_tap-9.3.8/vnpy_tap.egg-info/SOURCES.txt` & `vnpy_tap-9.3.9/vnpy_tap.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 vnpy_tap/api/TapQuoteAPI.dll
 vnpy_tap/api/__init__.py
 vnpy_tap/api/iTapTradeAPI_64.dll
 vnpy_tap/api/libTapDataCollectAPI.so
 vnpy_tap/api/libTapQuoteAPI.so
 vnpy_tap/api/libiTapTradeAPI.so
 vnpy_tap/api/tap_constant.py
+vnpy_tap/api/vntapmd.cp310-win_amd64.pyd
+vnpy_tap/api/vntaptd.cp310-win_amd64.pyd
 vnpy_tap/api/generator/tap_md_header_define.h
 vnpy_tap/api/generator/tap_md_header_function.h
 vnpy_tap/api/generator/tap_md_header_on.h
 vnpy_tap/api/generator/tap_md_header_process.h
 vnpy_tap/api/generator/tap_md_source_function.cpp
 vnpy_tap/api/generator/tap_md_source_module.cpp
 vnpy_tap/api/generator/tap_md_source_on.cpp
```

