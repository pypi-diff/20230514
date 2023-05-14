# Comparing `tmp/onvif-zeep-async-3.1.4.tar.gz` & `tmp/onvif-zeep-async-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-3.1.4.tar", last modified: Sun May 14 15:17:38 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.1.5.tar", last modified: Sun May 14 16:25:39 2023, max compression
```

## Comparing `onvif-zeep-async-3.1.4.tar` & `onvif-zeep-async-3.1.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.828806 onvif-zeep-async-3.1.4/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.4/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.4/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-14 15:17:38.828856 onvif-zeep-async-3.1.4/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.820098 onvif-zeep-async-3.1.4/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.821370 onvif-zeep-async-3.1.4/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    24999 2023-05-14 15:17:13.000000 onvif-zeep-async-3.1.4/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)    11738 2023-05-07 21:02:14.000000 onvif-zeep-async-3.1.4/onvif/managers.py
--rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/settings.py
--rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/transport.py
--rw-r--r--   0 bdraco     (501) staff       (20)      949 2023-05-14 15:17:13.000000 onvif-zeep-async-3.1.4/onvif/types.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3613 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-14 15:17:18.000000 onvif-zeep-async-3.1.4/onvif/version.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/wrappers.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.827687 onvif-zeep-async-3.1.4/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.828502 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1553 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       78 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-14 15:17:38.829074 onvif-zeep-async-3.1.4/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1859 2023-05-14 15:17:13.000000 onvif-zeep-async-3.1.4/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.828699 onvif-zeep-async-3.1.4/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/tests/test.py
--rw-r--r--   0 bdraco     (501) staff       (20)      291 2023-05-07 02:28:47.000000 onvif-zeep-async-3.1.4/tests/test_util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 16:25:39.093180 onvif-zeep-async-3.1.5/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.5/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.5/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-14 16:25:39.093230 onvif-zeep-async-3.1.5/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 16:25:39.083535 onvif-zeep-async-3.1.5/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 16:25:39.085128 onvif-zeep-async-3.1.5/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-05-14 16:23:24.000000 onvif-zeep-async-3.1.5/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    25030 2023-05-14 16:25:13.000000 onvif-zeep-async-3.1.5/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.5/onvif/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    11738 2023-05-07 21:02:14.000000 onvif-zeep-async-3.1.5/onvif/managers.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.5/onvif/settings.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.5/onvif/transport.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      949 2023-05-14 16:23:24.000000 onvif-zeep-async-3.1.5/onvif/types.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3613 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.5/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-14 16:25:18.000000 onvif-zeep-async-3.1.5/onvif/version.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.5/onvif/wrappers.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 16:25:39.092070 onvif-zeep-async-3.1.5/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 16:25:39.092854 onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-14 16:25:39.000000 onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1553 2023-05-14 16:25:39.000000 onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-14 16:25:39.000000 onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-14 16:25:39.000000 onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       78 2023-05-14 16:25:39.000000 onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-14 16:25:39.000000 onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-14 16:25:39.093473 onvif-zeep-async-3.1.5/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1859 2023-05-14 16:16:29.000000 onvif-zeep-async-3.1.5/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 16:25:39.093080 onvif-zeep-async-3.1.5/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.5/tests/test.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      291 2023-05-07 02:28:47.000000 onvif-zeep-async-3.1.5/tests/test_util.py
```

### Comparing `onvif-zeep-async-3.1.4/.gitignore` & `onvif-zeep-async-3.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/.pre-commit-config.yaml` & `onvif-zeep-async-3.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/LICENSE` & `onvif-zeep-async-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/Makefile` & `onvif-zeep-async-3.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/PKG-INFO` & `onvif-zeep-async-3.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.4
+Version: 3.1.5
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.4/README.rst` & `onvif-zeep-async-3.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/examples/events.py` & `onvif-zeep-async-3.1.5/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/examples/rotate_image.py` & `onvif-zeep-async-3.1.5/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/examples/streaming.py` & `onvif-zeep-async-3.1.5/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/__init__.py` & `onvif-zeep-async-3.1.5/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/client.py` & `onvif-zeep-async-3.1.5/onvif/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,17 @@
 async def _cached_document(url: str) -> Document:
     """Load external XML document from disk."""
     if url in _DOCUMENT_CACHE:
         return _DOCUMENT_CACHE[url]
     loop = asyncio.get_event_loop()
 
     def _load_document() -> DocumentWithDeferredLoad:
-        document = DocumentWithDeferredLoad(url, ASYNC_TRANSPORT, DEFAULT_SETTINGS)
+        document = DocumentWithDeferredLoad(
+            url, ASYNC_TRANSPORT, settings=DEFAULT_SETTINGS
+        )
         # Override the default datetime type to use FastDateTime
         # This is a workaround for the following issue:
         # https://github.com/mvantellingen/python-zeep/pull/1370
         schema = document.types.documents.get_by_namespace(
             "http://www.w3.org/2001/XMLSchema", False
         )[0]
         instance = FastDateTime(is_global=True)
```

### Comparing `onvif-zeep-async-3.1.4/onvif/definition.py` & `onvif-zeep-async-3.1.5/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/exceptions.py` & `onvif-zeep-async-3.1.5/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/managers.py` & `onvif-zeep-async-3.1.5/onvif/managers.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/transport.py` & `onvif-zeep-async-3.1.5/onvif/transport.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/types.py` & `onvif-zeep-async-3.1.5/onvif/types.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/util.py` & `onvif-zeep-async-3.1.5/onvif/util.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wrappers.py` & `onvif-zeep-async-3.1.5/onvif/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/addressing` & `onvif-zeep-async-3.1.5/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/envelope` & `onvif-zeep-async-3.1.5/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.1.5/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.1.5/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.1.5/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.4
+Version: 3.1.5
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.1.5/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/pylintrc` & `onvif-zeep-async-3.1.5/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/setup.py` & `onvif-zeep-async-3.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.4/tests/test.py` & `onvif-zeep-async-3.1.5/tests/test.py`

 * *Files identical despite different names*

