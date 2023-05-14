# Comparing `tmp/rpcclient-3.15.5.tar.gz` & `tmp/rpcclient-3.15.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-3.15.5.tar", last modified: Mon May  8 10:55:33 2023, max compression
+gzip compressed data, was "rpcclient-3.15.6.tar", last modified: Sun May 14 06:00:59 2023, max compression
```

## Comparing `rpcclient-3.15.5.tar` & `rpcclient-3.15.6.tar`

### file list

```diff
@@ -1,83 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-08 10:55:23.000000 rpcclient-3.15.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-08 10:55:33.732786 rpcclient-3.15.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 10:55:23.000000 rpcclient-3.15.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.728786 rpcclient-3.15.5/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.728786 rpcclient-3.15.5/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    37668 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.728786 rpcclient-3.15.5/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 10:55:33.732786 rpcclient-3.15.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-08 10:55:23.000000 rpcclient-3.15.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.399971 rpcclient-3.15.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-14 06:00:42.000000 rpcclient-3.15.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-05-14 06:00:59.399971 rpcclient-3.15.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-14 06:00:42.000000 rpcclient-3.15.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-14 06:00:42.000000 rpcclient-3.15.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-14 06:00:42.000000 rpcclient-3.15.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.391970 rpcclient-3.15.6/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.395970 rpcclient-3.15.6/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37668 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.395970 rpcclient-3.15.6/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.395970 rpcclient-3.15.6/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.399971 rpcclient-3.15.6/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.399971 rpcclient-3.15.6/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-14 06:00:42.000000 rpcclient-3.15.6/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.391970 rpcclient-3.15.6/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-05-14 06:00:59.000000 rpcclient-3.15.6/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-14 06:00:59.000000 rpcclient-3.15.6/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 06:00:59.000000 rpcclient-3.15.6/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 06:00:59.000000 rpcclient-3.15.6/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-14 06:00:59.000000 rpcclient-3.15.6/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-14 06:00:59.000000 rpcclient-3.15.6/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 06:00:59.399971 rpcclient-3.15.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:00:59.399971 rpcclient-3.15.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_allocation_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_core_foundation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_darwin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_objc_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_thread_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_worker_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-14 06:00:42.000000 rpcclient-3.15.6/tests/test_xpc.py
```

### Comparing `rpcclient-3.15.5/LICENSE` & `rpcclient-3.15.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/__main__.py` & `rpcclient-3.15.6/rpcclient/__main__.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/client.py` & `rpcclient-3.15.6/rpcclient/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/client_factory.py` & `rpcclient-3.15.6/rpcclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/bluetooth.py` & `rpcclient-3.15.6/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/cfpreferences.py` & `rpcclient-3.15.6/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/client.py` & `rpcclient-3.15.6/rpcclient/darwin/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/consts.py` & `rpcclient-3.15.6/rpcclient/darwin/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/core_graphics.py` & `rpcclient-3.15.6/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/crash_reports.py` & `rpcclient-3.15.6/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/darwin_lief.py` & `rpcclient-3.15.6/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/fs.py` & `rpcclient-3.15.6/rpcclient/darwin/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/hid.py` & `rpcclient-3.15.6/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/ioregistry.py` & `rpcclient-3.15.6/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/keychain.py` & `rpcclient-3.15.6/rpcclient/darwin/keychain.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/location.py` & `rpcclient-3.15.6/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/media.py` & `rpcclient-3.15.6/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/network.py` & `rpcclient-3.15.6/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/objc.py` & `rpcclient-3.15.6/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/objective_c_class.py` & `rpcclient-3.15.6/rpcclient/darwin/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-3.15.6/rpcclient/darwin/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/processes.py` & `rpcclient-3.15.6/rpcclient/darwin/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/reports.py` & `rpcclient-3.15.6/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/scpreferences.py` & `rpcclient-3.15.6/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/structs.py` & `rpcclient-3.15.6/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/symbol.py` & `rpcclient-3.15.6/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/syslog.py` & `rpcclient-3.15.6/rpcclient/darwin/syslog.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/time.py` & `rpcclient-3.15.6/rpcclient/darwin/time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/darwin/xpc.py` & `rpcclient-3.15.6/rpcclient/darwin/xpc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/exceptions.py` & `rpcclient-3.15.6/rpcclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/fs.py` & `rpcclient-3.15.6/rpcclient/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/accessibility.py` & `rpcclient-3.15.6/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/amfi.py` & `rpcclient-3.15.6/rpcclient/ios/amfi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/backlight.py` & `rpcclient-3.15.6/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/client.py` & `rpcclient-3.15.6/rpcclient/ios/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/lockdown.py` & `rpcclient-3.15.6/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/mobile_gestalt.py` & `rpcclient-3.15.6/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/screen_capture.py` & `rpcclient-3.15.6/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/sprinboard.py` & `rpcclient-3.15.6/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/telephony.py` & `rpcclient-3.15.6/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/ios/wifi.py` & `rpcclient-3.15.6/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/lief.py` & `rpcclient-3.15.6/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/linux/client.py` & `rpcclient-3.15.6/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/linux/structs.py` & `rpcclient-3.15.6/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/macos/apple_script.py` & `rpcclient-3.15.6/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/macos/client.py` & `rpcclient-3.15.6/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/network.py` & `rpcclient-3.15.6/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/processes.py` & `rpcclient-3.15.6/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/protocol.py` & `rpcclient-3.15.6/rpcclient/protocol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/structs/consts.py` & `rpcclient-3.15.6/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/structs/generic.py` & `rpcclient-3.15.6/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/symbol.py` & `rpcclient-3.15.6/rpcclient/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/symbols_jar.py` & `rpcclient-3.15.6/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/sysctl.py` & `rpcclient-3.15.6/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient/xonshrc.py` & `rpcclient-3.15.6/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.5/rpcclient.egg-info/SOURCES.txt` & `rpcclient-3.15.6/rpcclient.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
+requirements.txt
 rpcclient/__init__.py
 rpcclient/__main__.py
 rpcclient/allocated.py
 rpcclient/client.py
 rpcclient/client_factory.py
 rpcclient/exceptions.py
 rpcclient/fs.py
@@ -66,8 +67,23 @@
 rpcclient/linux/client.py
 rpcclient/linux/structs.py
 rpcclient/macos/__init__.py
 rpcclient/macos/apple_script.py
 rpcclient/macos/client.py
 rpcclient/structs/__init__.py
 rpcclient/structs/consts.py
-rpcclient/structs/generic.py
+rpcclient/structs/generic.py
+tests/test_allocation_cleanup.py
+tests/test_client.py
+tests/test_core_foundation_types.py
+tests/test_darwin_client.py
+tests/test_fs.py
+tests/test_keychain.py
+tests/test_objc_symbol.py
+tests/test_preferences.py
+tests/test_processes.py
+tests/test_socket.py
+tests/test_spawn.py
+tests/test_thread_safe.py
+tests/test_time.py
+tests/test_worker_processes.py
+tests/test_xpc.py
```

