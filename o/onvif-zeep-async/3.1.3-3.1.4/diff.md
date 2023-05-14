# Comparing `tmp/onvif-zeep-async-3.1.3.tar.gz` & `tmp/onvif-zeep-async-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-3.1.3.tar", last modified: Tue May  9 23:36:04 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.1.4.tar", last modified: Sun May 14 15:17:38 2023, max compression
```

## Comparing `onvif-zeep-async-3.1.3.tar` & `onvif-zeep-async-3.1.4.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-09 23:36:04.423343 onvif-zeep-async-3.1.3/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.3/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.3/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-09 23:36:04.423394 onvif-zeep-async-3.1.3/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-09 23:36:04.412786 onvif-zeep-async-3.1.3/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-09 23:36:04.414899 onvif-zeep-async-3.1.3/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    23790 2023-05-09 23:30:56.000000 onvif-zeep-async-3.1.3/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.3/onvif/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)    11738 2023-05-07 21:02:14.000000 onvif-zeep-async-3.1.3/onvif/managers.py
--rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.3/onvif/settings.py
--rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.3/onvif/transport.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3613 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.3/onvif/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-09 23:31:00.000000 onvif-zeep-async-3.1.3/onvif/version.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.3/onvif/wrappers.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-09 23:36:04.421951 onvif-zeep-async-3.1.3/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-09 23:36:04.422889 onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-09 23:36:04.000000 onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1538 2023-05-09 23:36:04.000000 onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-09 23:36:04.000000 onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-09 23:36:04.000000 onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-09 23:36:04.000000 onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-09 23:36:04.000000 onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-09 23:36:04.423617 onvif-zeep-async-3.1.3/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.1.3/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-09 23:36:04.423111 onvif-zeep-async-3.1.3/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.3/tests/test.py
--rw-r--r--   0 bdraco     (501) staff       (20)      291 2023-05-07 02:28:47.000000 onvif-zeep-async-3.1.3/tests/test_util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.828806 onvif-zeep-async-3.1.4/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.4/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.4/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-14 15:17:38.828856 onvif-zeep-async-3.1.4/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.820098 onvif-zeep-async-3.1.4/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.821370 onvif-zeep-async-3.1.4/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    24999 2023-05-14 15:17:13.000000 onvif-zeep-async-3.1.4/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    11738 2023-05-07 21:02:14.000000 onvif-zeep-async-3.1.4/onvif/managers.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/settings.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/transport.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      949 2023-05-14 15:17:13.000000 onvif-zeep-async-3.1.4/onvif/types.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3613 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-14 15:17:18.000000 onvif-zeep-async-3.1.4/onvif/version.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.4/onvif/wrappers.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.827687 onvif-zeep-async-3.1.4/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.828502 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1553 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       78 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-14 15:17:38.000000 onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-14 15:17:38.829074 onvif-zeep-async-3.1.4/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1859 2023-05-14 15:17:13.000000 onvif-zeep-async-3.1.4/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 15:17:38.828699 onvif-zeep-async-3.1.4/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.4/tests/test.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      291 2023-05-07 02:28:47.000000 onvif-zeep-async-3.1.4/tests/test_util.py
```

### Comparing `onvif-zeep-async-3.1.3/.gitignore` & `onvif-zeep-async-3.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/.pre-commit-config.yaml` & `onvif-zeep-async-3.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/LICENSE` & `onvif-zeep-async-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/Makefile` & `onvif-zeep-async-3.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/PKG-INFO` & `onvif-zeep-async-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.3
+Version: 3.1.4
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.3/README.rst` & `onvif-zeep-async-3.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/examples/events.py` & `onvif-zeep-async-3.1.4/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/examples/rotate_image.py` & `onvif-zeep-async-3.1.4/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/examples/streaming.py` & `onvif-zeep-async-3.1.4/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/__init__.py` & `onvif-zeep-async-3.1.4/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/client.py` & `onvif-zeep-async-3.1.4/onvif/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from onvif.definition import SERVICES
 from onvif.exceptions import ONVIFAuthError, ONVIFError, ONVIFTimeoutError
 
 from .const import KEEPALIVE_EXPIRY
 from .managers import NotificationManager, PullPointManager
 from .settings import DEFAULT_SETTINGS
 from .transport import ASYNC_TRANSPORT
+from .types import FastDateTime
 from .util import create_no_verify_ssl_context, normalize_url, path_isfile, utcnow
 from .wrappers import retry_connection_error  # noqa: F401
 
 logger = logging.getLogger("onvif")
 logging.basicConfig(level=logging.INFO)
 logging.getLogger("zeep.client").setLevel(logging.CRITICAL)
 
@@ -76,18 +77,52 @@
         if self.dt_diff is not None:
             self.created += self.dt_diff
         result = super().apply(envelope, headers)
         self.created = old_created
         return result
 
 
-@lru_cache(maxsize=128)
-def _cached_document(url: str) -> Document:
+_DOCUMENT_CACHE: dict[str, Document] = {}
+
+original_load = Document.load
+
+
+class DocumentWithDeferredLoad(Document):
+    def load(self, *args: Any, **kwargs: Any) -> None:
+        """Deferred load of the document."""
+
+    def original_load(self, *args: Any, **kwargs: Any) -> None:
+        """Original load of the document."""
+        return original_load(self, *args, **kwargs)
+
+
+async def _cached_document(url: str) -> Document:
     """Load external XML document from disk."""
-    return Document(url, ASYNC_TRANSPORT, settings=DEFAULT_SETTINGS)
+    if url in _DOCUMENT_CACHE:
+        return _DOCUMENT_CACHE[url]
+    loop = asyncio.get_event_loop()
+
+    def _load_document() -> DocumentWithDeferredLoad:
+        document = DocumentWithDeferredLoad(url, ASYNC_TRANSPORT, DEFAULT_SETTINGS)
+        # Override the default datetime type to use FastDateTime
+        # This is a workaround for the following issue:
+        # https://github.com/mvantellingen/python-zeep/pull/1370
+        schema = document.types.documents.get_by_namespace(
+            "http://www.w3.org/2001/XMLSchema", False
+        )[0]
+        instance = FastDateTime(is_global=True)
+        schema.register_type(FastDateTime._default_qname, instance)
+        document.types.add_documents([None], url)
+        # Perform the original load
+        document.original_load(url)
+        return document
+
+    document = await loop.run_in_executor(None, _load_document)
+    _DOCUMENT_CACHE[url] = document
+    return document
 
 
 class ZeepAsyncClient(BaseZeepAsyncClient):
     """Overwrite create_service method to be async."""
 
     def create_service(self, binding_name, address):
         """Create a new ServiceProxy for the given binding name and address.
@@ -197,17 +232,15 @@
     async def setup(self):
         """Setup the transport."""
         settings = DEFAULT_SETTINGS
         binding_name = self.binding_name
         wsse = UsernameDigestTokenDtDiff(
             self.user, self.passwd, dt_diff=self.dt_diff, use_digest=self.encrypt
         )
-        self.document = await self.loop.run_in_executor(
-            None, _cached_document, self.url
-        )
+        self.document = await _cached_document(self.url)
         self.zeep_client_authless = ZeepAsyncClient(
             wsdl=self.document,
             transport=self.transport,
             settings=settings,
             plugins=[WsAddressingPlugin()],
         )
         self.ws_client_authless = self.zeep_client_authless.create_service(
```

### Comparing `onvif-zeep-async-3.1.3/onvif/definition.py` & `onvif-zeep-async-3.1.4/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/exceptions.py` & `onvif-zeep-async-3.1.4/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/managers.py` & `onvif-zeep-async-3.1.4/onvif/managers.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/transport.py` & `onvif-zeep-async-3.1.4/onvif/transport.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/util.py` & `onvif-zeep-async-3.1.4/onvif/util.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wrappers.py` & `onvif-zeep-async-3.1.4/onvif/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/addressing` & `onvif-zeep-async-3.1.4/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/envelope` & `onvif-zeep-async-3.1.4/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.1.4/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.1.4/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.1.4/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.3
+Version: 3.1.4
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.3/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.1.4/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 onvif/client.py
 onvif/const.py
 onvif/definition.py
 onvif/exceptions.py
 onvif/managers.py
 onvif/settings.py
 onvif/transport.py
+onvif/types.py
 onvif/util.py
 onvif/version.txt
 onvif/wrappers.py
 onvif/wsdl/__init__.py
 onvif/wsdl/accesscontrol.wsdl
 onvif/wsdl/actionengine.wsdl
 onvif/wsdl/addressing
```

### Comparing `onvif-zeep-async-3.1.3/pylintrc` & `onvif-zeep-async-3.1.4/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.3/setup.py` & `onvif-zeep-async-3.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 version_path = os.path.join(here, "onvif/version.txt")
 version = open(version_path).read().strip()
 
-requires = ["httpx>=0.19.0,<1.0.0", "zeep[async]>=4.2.1,<5.0.0"]
+requires = [
+    "httpx>=0.19.0,<1.0.0",
+    "zeep[async]>=4.2.1,<5.0.0",
+    "ciso8601>=2.1.3",
+    "isodate>=0.6.0",
+]
 
 CLASSIFIERS = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Customer Service",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
```

### Comparing `onvif-zeep-async-3.1.3/tests/test.py` & `onvif-zeep-async-3.1.4/tests/test.py`

 * *Files identical despite different names*

