# Comparing `tmp/p4p-4.1.5a1.tar.gz` & `tmp/p4p-4.1.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4p-4.1.5a1.tar", last modified: Mon Nov 28 04:48:35 2022, max compression
+gzip compressed data, was "p4p-4.1.6a1.tar", last modified: Sun May 14 16:34:40 2023, max compression
```

## Comparing `p4p-4.1.5a1.tar` & `p4p-4.1.6a1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.542331 p4p-4.1.5a1/
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2022-11-28 04:48:05.000000 p4p-4.1.5a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      237 2022-11-28 04:48:05.000000 p4p-4.1.5a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2022-11-28 04:48:35.542331 p4p-4.1.5a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      440 2022-11-28 04:48:05.000000 p4p-4.1.5a1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-11-28 04:48:05.000000 p4p-4.1.5a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 04:48:35.542331 p4p-4.1.5a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     4846 2022-11-28 04:48:05.000000 p4p-4.1.5a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.534331 p4p-4.1.5a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.538331 p4p-4.1.5a1/src/p4p/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11839 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/_gw.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      389 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/_p4p.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    27324 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/_p4p.pyx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.538331 p4p-4.1.5a1/src/p4p/asLib/
--rw-r--r--   0 runner    (1001) docker     (122)    10110 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/asLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/asLib/lex.py
--rw-r--r--   0 runner    (1001) docker     (122)     5326 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/asLib/pvlist.py
--rw-r--r--   0 runner    (1001) docker     (122)     2403 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/asLib/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.538331 p4p-4.1.5a1/src/p4p/client/
--rw-r--r--   0 runner    (1001) docker     (122)    10653 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/client/Qt.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14557 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/client/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)     4090 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/client/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    11841 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/client/cothread.py
--rw-r--r--   0 runner    (1001) docker     (122)     9418 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/client/raw.py
--rw-r--r--   0 runner    (1001) docker     (122)    15778 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/client/thread.py
--rw-r--r--   0 runner    (1001) docker     (122)     4211 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/disect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/example.conf
--rw-r--r--   0 runner    (1001) docker     (122)    28038 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/gw.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.538331 p4p-4.1.5a1/src/p4p/nt/
--rw-r--r--   0 runner    (1001) docker     (122)     8522 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/nt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2401 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/nt/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/nt/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     6597 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/nt/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (122)     7681 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/nt/scalar.py
--rw-r--r--   0 runner    (1001) docker     (122)      604 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvagw@.service
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.538331 p4p-4.1.5a1/src/p4p/pvxs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/client.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     6323 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/data.pxd
--rw-r--r--   0 runner    (1001) docker     (122)      401 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/log.pxd
--rw-r--r--   0 runner    (1001) docker     (122)      329 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/nt.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/server.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1652 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/sharedArray.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/sharedpv.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/source.pxd
--rw-r--r--   0 runner    (1001) docker     (122)      384 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/util.pxd
--rw-r--r--   0 runner    (1001) docker     (122)      292 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/pvxs/version.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.542331 p4p-4.1.5a1/src/p4p/server/
--rw-r--r--   0 runner    (1001) docker     (122)     8516 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3718 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/server/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)     2884 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/server/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     3704 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/server/cothread.py
--rw-r--r--   0 runner    (1001) docker     (122)     8411 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/server/raw.py
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/server/thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      713 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/set.pxd
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.542331 p4p-4.1.5a1/src/p4p/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8252 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/asynciotest.py
--rw-r--r--   0 runner    (1001) docker     (122)     7691 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/cothreadtest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2920 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/qttest.py
--rw-r--r--   0 runner    (1001) docker     (122)    11051 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_asLib.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)     3186 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_client_raw.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_client_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      241 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_cothread.py
--rw-r--r--   0 runner    (1001) docker     (122)    20146 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_gw.py
--rw-r--r--   0 runner    (1001) docker     (122)    11754 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_nt.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (122)    12615 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_sharedpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     4438 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    18905 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/test_value.py
--rw-r--r--   0 runner    (1001) docker     (122)     5456 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     6906 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:48:35.538331 p4p-4.1.5a1/src/p4p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2022-11-28 04:48:35.000000 p4p-4.1.5a1/src/p4p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2022-11-28 04:48:35.000000 p4p-4.1.5a1/src/p4p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:48:35.000000 p4p-4.1.5a1/src/p4p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2022-11-28 04:48:35.000000 p4p-4.1.5a1/src/p4p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:48:35.000000 p4p-4.1.5a1/src/p4p.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      109 2022-11-28 04:48:35.000000 p4p-4.1.5a1/src/p4p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2022-11-28 04:48:35.000000 p4p-4.1.5a1/src/p4p.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4993 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/p4p.h
--rw-r--r--   0 runner    (1001) docker     (122)     3120 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/pvxs_client.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    29811 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/pvxs_gw.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4871 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/pvxs_gw.h
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/pvxs_odometer.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3322 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/pvxs_sharedpv.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/pvxs_source.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5100 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/pvxs_type.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    17719 2022-11-28 04:48:05.000000 p4p-4.1.5a1/src/pvxs_value.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.875988 p4p-4.1.6a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-14 16:33:50.000000 p4p-4.1.6a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-14 16:33:50.000000 p4p-4.1.6a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-14 16:34:40.875988 p4p-4.1.6a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-14 16:33:50.000000 p4p-4.1.6a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-14 16:33:50.000000 p4p-4.1.6a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:34:40.875988 p4p-4.1.6a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-05-14 16:33:50.000000 p4p-4.1.6a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.863988 p4p-4.1.6a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.867988 p4p-4.1.6a1/src/p4p/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/_gw.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/_p4p.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    27324 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/_p4p.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.867988 p4p-4.1.6a1/src/p4p/asLib/
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/asLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/asLib/lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/asLib/pvlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/asLib/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.871988 p4p-4.1.6a1/src/p4p/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/client/Qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/client/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/client/cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/client/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/client/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/disect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/example.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/gw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.871988 p4p-4.1.6a1/src/p4p/nt/
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/nt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/nt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/nt/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/nt/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/nt/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvagw@.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.871988 p4p-4.1.6a1/src/p4p/pvxs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/client.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/log.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/nt.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/server.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/sharedArray.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/sharedpv.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/source.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/pvxs/version.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.871988 p4p-4.1.6a1/src/p4p/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/server/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/server/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/server/cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/server/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/server/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/set.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.875988 p4p-4.1.6a1/src/p4p/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/asynciotest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/cothreadtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/qttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_asLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_client_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_client_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_sharedpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:40.867988 p4p-4.1.6a1/src/p4p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-14 16:34:40.000000 p4p-4.1.6a1/src/p4p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-14 16:34:40.000000 p4p-4.1.6a1/src/p4p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:34:40.000000 p4p-4.1.6a1/src/p4p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 16:34:40.000000 p4p-4.1.6a1/src/p4p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:34:40.000000 p4p-4.1.6a1/src/p4p.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-14 16:34:40.000000 p4p-4.1.6a1/src/p4p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-14 16:34:40.000000 p4p-4.1.6a1/src/p4p.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/p4p.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/pvxs_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/pvxs_gw.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/pvxs_gw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/pvxs_odometer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/pvxs_sharedpv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/pvxs_source.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/pvxs_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17719 2023-05-14 16:33:50.000000 p4p-4.1.6a1/src/pvxs_value.cpp
```

### Comparing `p4p-4.1.5a1/LICENSE` & `p4p-4.1.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/PKG-INFO` & `p4p-4.1.6a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4p
-Version: 4.1.5a1
+Version: 4.1.6a1
 Summary: Python interface to PVAccess protocol client
 Home-page: https://mdavidsaver.github.io/p4p
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Keywords: epics scada
 Platform: UNKNOWN
```

### Comparing `p4p-4.1.5a1/setup.py` & `p4p-4.1.6a1/setup.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/__init__.py` & `p4p-4.1.6a1/src/p4p/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/_gw.pyx` & `p4p-4.1.6a1/src/p4p/_gw.pyx`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/_p4p.pyx` & `p4p-4.1.6a1/src/p4p/_p4p.pyx`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/asLib/__init__.py` & `p4p-4.1.6a1/src/p4p/asLib/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/asLib/lex.py` & `p4p-4.1.6a1/src/p4p/asLib/lex.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/asLib/pvlist.py` & `p4p-4.1.6a1/src/p4p/asLib/pvlist.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/asLib/yacc.py` & `p4p-4.1.6a1/src/p4p/asLib/yacc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/client/Qt.py` & `p4p-4.1.6a1/src/p4p/client/Qt.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/client/asyncio.py` & `p4p-4.1.6a1/src/p4p/client/asyncio.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/client/cli.py` & `p4p-4.1.6a1/src/p4p/client/cli.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/client/cothread.py` & `p4p-4.1.6a1/src/p4p/client/cothread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/client/raw.py` & `p4p-4.1.6a1/src/p4p/client/raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/client/thread.py` & `p4p-4.1.6a1/src/p4p/client/thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/disect.py` & `p4p-4.1.6a1/src/p4p/disect.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/example.conf` & `p4p-4.1.6a1/src/p4p/example.conf`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/gw.py` & `p4p-4.1.6a1/src/p4p/gw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/nt/__init__.py` & `p4p-4.1.6a1/src/p4p/nt/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/nt/common.py` & `p4p-4.1.6a1/src/p4p/nt/common.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/nt/enum.py` & `p4p-4.1.6a1/src/p4p/nt/enum.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/nt/ndarray.py` & `p4p-4.1.6a1/src/p4p/nt/ndarray.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/nt/scalar.py` & `p4p-4.1.6a1/src/p4p/nt/scalar.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/pvagw@.service` & `p4p-4.1.6a1/src/p4p/pvagw@.service`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/pvxs/client.pxd` & `p4p-4.1.6a1/src/p4p/pvxs/client.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/pvxs/data.pxd` & `p4p-4.1.6a1/src/p4p/pvxs/data.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/pvxs/server.pxd` & `p4p-4.1.6a1/src/p4p/pvxs/server.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/pvxs/sharedArray.pxd` & `p4p-4.1.6a1/src/p4p/pvxs/sharedArray.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/pvxs/sharedpv.pxd` & `p4p-4.1.6a1/src/p4p/pvxs/sharedpv.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/pvxs/source.pxd` & `p4p-4.1.6a1/src/p4p/pvxs/source.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/rpc.py` & `p4p-4.1.6a1/src/p4p/rpc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/server/__init__.py` & `p4p-4.1.6a1/src/p4p/server/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/server/asyncio.py` & `p4p-4.1.6a1/src/p4p/server/asyncio.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/server/cli.py` & `p4p-4.1.6a1/src/p4p/server/cli.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/server/cothread.py` & `p4p-4.1.6a1/src/p4p/server/cothread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/server/raw.py` & `p4p-4.1.6a1/src/p4p/server/raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/server/thread.py` & `p4p-4.1.6a1/src/p4p/server/thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/set.pxd` & `p4p-4.1.6a1/src/p4p/set.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/asynciotest.py` & `p4p-4.1.6a1/src/p4p/test/asynciotest.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,24 +116,25 @@
 
                     self.assertEqual(3, (await Q.get()))
 
                 finally:
                     sub.close()
                     await sub.wait_closed()
 
-    @asyncio.coroutine
-    def test_gen_coro(self):
-        # demonstrate interoperability w/ code using generated based coroutines
-        with Server(providers=[self.provider], isolate=True) as S:
-            with Context('pva', conf=S.conf(), useenv=False) as C:
-                self.assertEqual(0, (yield from C.get('foo')))
+    if hasattr(asyncio, 'coroutine'):
+        @asyncio.coroutine
+        def test_gen_coro(self):
+            # demonstrate interoperability w/ code using generated based coroutines
+            with Server(providers=[self.provider], isolate=True) as S:
+                with Context('pva', conf=S.conf(), useenv=False) as C:
+                    self.assertEqual(0, (yield from C.get('foo')))
 
-                yield from C.put('foo', 5)
+                    yield from C.put('foo', 5)
 
-                self.assertEqual(5 * 2, (yield from C.get('foo')))
+                    self.assertEqual(5 * 2, (yield from C.get('foo')))
 
 
 class TestTimeout(AsyncTest):
 
     async def test_timeout(self):
         done = None
```

### Comparing `p4p-4.1.5a1/src/p4p/test/cothreadtest.py` & `p4p-4.1.6a1/src/p4p/test/cothreadtest.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/qttest.py` & `p4p-4.1.6a1/src/p4p/test/qttest.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_asLib.py` & `p4p-4.1.6a1/src/p4p/test/test_asLib.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_client_raw.py` & `p4p-4.1.6a1/src/p4p/test/test_client_raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_client_thread.py` & `p4p-4.1.6a1/src/p4p/test/test_client_thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_gw.py` & `p4p-4.1.6a1/src/p4p/test/test_gw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_nt.py` & `p4p-4.1.6a1/src/p4p/test/test_nt.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_rpc.py` & `p4p-4.1.6a1/src/p4p/test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_server.py` & `p4p-4.1.6a1/src/p4p/test/test_server.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_sharedpv.py` & `p4p-4.1.6a1/src/p4p/test/test_sharedpv.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_type.py` & `p4p-4.1.6a1/src/p4p/test/test_type.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/test_value.py` & `p4p-4.1.6a1/src/p4p/test/test_value.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/test/utils.py` & `p4p-4.1.6a1/src/p4p/test/utils.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/util.py` & `p4p-4.1.6a1/src/p4p/util.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p/version.py` & `p4p-4.1.6a1/src/p4p/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,8 +63,8 @@
     def __eq__(self, o):
         return self._cmp(o)==0
     def __ge__(self, o):
         return self._cmp(o)>=0
     def __gt__(self, o):
         return self._cmp(o)>0
 
-version = Version('4.1.5a1')
+version = Version('4.1.6a1')
```

### Comparing `p4p-4.1.5a1/src/p4p/wrapper.py` & `p4p-4.1.6a1/src/p4p/wrapper.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p.egg-info/PKG-INFO` & `p4p-4.1.6a1/src/p4p.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4p
-Version: 4.1.5a1
+Version: 4.1.6a1
 Summary: Python interface to PVAccess protocol client
 Home-page: https://mdavidsaver.github.io/p4p
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Keywords: epics scada
 Platform: UNKNOWN
```

### Comparing `p4p-4.1.5a1/src/p4p.egg-info/SOURCES.txt` & `p4p-4.1.6a1/src/p4p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/p4p.h` & `p4p-4.1.6a1/src/p4p.h`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/pvxs_client.cpp` & `p4p-4.1.6a1/src/pvxs_client.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/pvxs_gw.cpp` & `p4p-4.1.6a1/src/pvxs_gw.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/pvxs_gw.h` & `p4p-4.1.6a1/src/pvxs_gw.h`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/pvxs_odometer.cpp` & `p4p-4.1.6a1/src/pvxs_odometer.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/pvxs_sharedpv.cpp` & `p4p-4.1.6a1/src/pvxs_sharedpv.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/pvxs_source.cpp` & `p4p-4.1.6a1/src/pvxs_source.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/pvxs_type.cpp` & `p4p-4.1.6a1/src/pvxs_type.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.5a1/src/pvxs_value.cpp` & `p4p-4.1.6a1/src/pvxs_value.cpp`

 * *Files identical despite different names*

