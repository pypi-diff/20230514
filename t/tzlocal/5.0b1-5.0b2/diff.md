# Comparing `tmp/tzlocal-5.0b1.tar.gz` & `tmp/tzlocal-5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tzlocal-5.0b1.tar", last modified: Fri Apr  7 10:20:33 2023, max compression
+gzip compressed data, was "tzlocal-5.0b2.tar", last modified: Tue Apr 11 14:39:46 2023, max compression
```

## Comparing `tzlocal-5.0b1.tar` & `tzlocal-5.0b2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.781944 tzlocal-5.0b1/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8092 2023-04-07 10:20:33.000000 tzlocal-5.0b1/CHANGES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1060 2023-04-07 10:20:33.000000 tzlocal-5.0b1/LICENSE.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      113 2023-04-07 10:20:33.000000 tzlocal-5.0b1/MANIFEST.in
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    15084 2023-04-07 10:20:33.781944 tzlocal-5.0b1/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5961 2023-04-07 10:20:33.000000 tzlocal-5.0b1/README.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      143 2023-04-07 10:20:33.000000 tzlocal-5.0b1/pyproject.toml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1316 2023-04-07 10:20:33.781944 tzlocal-5.0b1/setup.cfg
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-04-07 10:20:33.000000 tzlocal-5.0b1/setup.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/Africa/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/Africa/Harare
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/UTC
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/conflicting/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/conflicting/etc/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/conflicting/etc/conf.d/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       33 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/conflicting/etc/conf.d/clock
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/conflicting/etc/localtime
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/conflicting/etc/sysconfig/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/conflicting/etc/sysconfig/clock
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       64 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/conflicting/etc/timezone
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/conflicting/usr/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/conflicting/usr/share/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/conflicting/usr/share/zoneinfo/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/conflicting/usr/share/zoneinfo/Africa/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/conflicting/usr/share/zoneinfo/Africa/Harare
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/conflicting/var/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/conflicting/var/db/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       83 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/conflicting/var/db/zoneinfo
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/localtime/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/localtime/etc/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/localtime/etc/localtime
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/noconflict/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/noconflict/etc/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/noconflict/etc/conf.d/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/noconflict/etc/conf.d/clock
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/noconflict/etc/localtime
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/noconflict/etc/sysconfig/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       12 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/noconflict/etc/sysconfig/clock
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       59 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/noconflict/etc/timezone
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/noconflict/usr/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/noconflict/usr/share/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/noconflict/usr/share/zoneinfo/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/noconflict/usr/share/zoneinfo/Etc/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/noconflict/usr/share/zoneinfo/Etc/UCT
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/noconflict/usr/share/zoneinfo/Etc/UTC
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/noconflict/usr/share/zoneinfo/UTC
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/noconflict/usr/share/zoneinfo/Zulu
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/symlink_localtime/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/symlink_localtime/etc/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/symlink_localtime/etc/localtime
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/symlink_localtime/usr/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/symlink_localtime/usr/share/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.773944 tzlocal-5.0b1/tests/test_data/symlink_localtime/usr/share/zoneinfo/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/symlink_localtime/usr/share/zoneinfo/Africa/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/symlink_localtime/usr/share/zoneinfo/Africa/Harare
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/termux/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/termux/system/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/termux/system/bin/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       68 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/termux/system/bin/getprop
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/timezone/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/timezone/etc/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       65 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/timezone/etc/timezone
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/timezone_setting/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/timezone_setting/etc/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/timezone_setting/etc/conf.d/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       27 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/timezone_setting/etc/conf.d/clock
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/top_line_comment/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/top_line_comment/etc/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/top_line_comment/etc/timezone
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/ubuntu_docker_bug/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/ubuntu_docker_bug/etc/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        5 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/ubuntu_docker_bug/etc/timezone
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/vardbzoneinfo/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/vardbzoneinfo/etc/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/vardbzoneinfo/etc/timezone
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/vardbzoneinfo/var/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.781944 tzlocal-5.0b1/tests/test_data/vardbzoneinfo/var/db/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       80 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/vardbzoneinfo/var/db/zoneinfo
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/zone_setting/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.777944 tzlocal-5.0b1/tests/test_data/zone_setting/etc/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.781944 tzlocal-5.0b1/tests/test_data/zone_setting/etc/sysconfig/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_data/zone_setting/etc/sysconfig/clock
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10284 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tests/test_tzlocal.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.781944 tzlocal-5.0b1/tzlocal/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      334 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8098 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal/unix.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3880 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal/utils.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4665 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal/win32.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    34203 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal/windows_tz.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-07 10:20:33.781944 tzlocal-5.0b1/tzlocal.egg-info/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    15084 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal.egg-info/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1629 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal.egg-info/SOURCES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal.egg-info/dependency_links.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      185 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal.egg-info/requires.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        8 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal.egg-info/top_level.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-07 10:20:33.000000 tzlocal-5.0b1/tzlocal.egg-info/zip-safe
--rwxrwxr-x   0 lregebro  (1000) lregebro  (1000)     3318 2023-04-07 10:20:33.000000 tzlocal-5.0b1/update_windows_mappings.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8486 2023-04-11 14:39:46.000000 tzlocal-5.0b2/CHANGES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1060 2023-04-11 14:39:46.000000 tzlocal-5.0b2/LICENSE.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      113 2023-04-11 14:39:46.000000 tzlocal-5.0b2/MANIFEST.in
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    15478 2023-04-11 14:39:46.993866 tzlocal-5.0b2/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5961 2023-04-11 14:39:46.000000 tzlocal-5.0b2/README.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      143 2023-04-11 14:39:46.000000 tzlocal-5.0b2/pyproject.toml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1316 2023-04-11 14:39:46.993866 tzlocal-5.0b2/setup.cfg
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-04-11 14:39:46.000000 tzlocal-5.0b2/setup.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/Africa/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/Africa/Harare
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/UTC
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/conflicting/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/conflicting/etc/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/conflicting/etc/conf.d/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       33 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/conflicting/etc/conf.d/clock
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/conflicting/etc/localtime
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/conflicting/etc/sysconfig/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/conflicting/etc/sysconfig/clock
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       64 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/conflicting/etc/timezone
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/conflicting/usr/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/conflicting/usr/share/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/conflicting/usr/share/zoneinfo/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/conflicting/usr/share/zoneinfo/Africa/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/conflicting/usr/share/zoneinfo/Africa/Harare
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/conflicting/var/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/conflicting/var/db/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       83 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/conflicting/var/db/zoneinfo
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/localtime/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/localtime/etc/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/localtime/etc/localtime
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/noconflict/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/noconflict/etc/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/noconflict/etc/conf.d/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/noconflict/etc/conf.d/clock
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/noconflict/etc/localtime
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/noconflict/etc/sysconfig/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       12 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/noconflict/etc/sysconfig/clock
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       59 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/noconflict/etc/timezone
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/noconflict/usr/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/noconflict/usr/share/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/noconflict/usr/share/zoneinfo/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/noconflict/usr/share/zoneinfo/Etc/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/noconflict/usr/share/zoneinfo/Etc/UCT
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/noconflict/usr/share/zoneinfo/Etc/UTC
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/noconflict/usr/share/zoneinfo/UTC
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      118 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/noconflict/usr/share/zoneinfo/Zulu
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/symlink_localtime/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/symlink_localtime/etc/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/symlink_localtime/etc/localtime
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/symlink_localtime/usr/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/symlink_localtime/usr/share/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/symlink_localtime/usr/share/zoneinfo/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/symlink_localtime/usr/share/zoneinfo/Africa/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      157 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/symlink_localtime/usr/share/zoneinfo/Africa/Harare
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/termux/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/termux/system/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/termux/system/bin/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       68 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/termux/system/bin/getprop
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/timezone/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/timezone/etc/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       65 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/timezone/etc/timezone
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/timezone_setting/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/timezone_setting/etc/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/timezone_setting/etc/conf.d/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       27 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/timezone_setting/etc/conf.d/clock
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/top_line_comment/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/top_line_comment/etc/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/top_line_comment/etc/timezone
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/ubuntu_docker_bug/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/ubuntu_docker_bug/etc/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        5 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/ubuntu_docker_bug/etc/timezone
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/vardbzoneinfo/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/vardbzoneinfo/etc/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/vardbzoneinfo/etc/timezone
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/vardbzoneinfo/var/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/vardbzoneinfo/var/db/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       80 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/vardbzoneinfo/var/db/zoneinfo
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/zone_setting/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.985866 tzlocal-5.0b2/tests/test_data/zone_setting/etc/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tests/test_data/zone_setting/etc/sysconfig/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_data/zone_setting/etc/sysconfig/clock
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10465 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tests/test_tzlocal.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tzlocal/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      417 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8111 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal/unix.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3313 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal/utils.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4691 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal/win32.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    34203 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal/windows_tz.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-11 14:39:46.989866 tzlocal-5.0b2/tzlocal.egg-info/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    15478 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal.egg-info/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1629 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal.egg-info/SOURCES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal.egg-info/dependency_links.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      185 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal.egg-info/requires.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        8 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal.egg-info/top_level.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-11 14:39:46.000000 tzlocal-5.0b2/tzlocal.egg-info/zip-safe
+-rwxrwxr-x   0 lregebro  (1000) lregebro  (1000)     3318 2023-04-11 14:39:46.000000 tzlocal-5.0b2/update_windows_mappings.py
```

### Comparing `tzlocal-5.0b1/CHANGES.txt` & `tzlocal-5.0b2/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Changes
 =======
 
+5.0b2 (2023-04-11)
+------------------
+
+- Change how the system offset is calculated to deal with non-DST
+  temporary changes, such as Ramadan time in Morocco.
+
+- Change the default to only warn when the timezone offset and system
+  offset disagree (but still not even warn if TZ is set)
+
+- Add the assert_tz_offset() method to the top level for those who want
+  to explicitly check and fail.
+
+
 5.0b1 (2023-04-07)
 ------------------
 
 - Removed the deprecation shim. 
 
 
 4.4b1 (2023-03-20)
```

### Comparing `tzlocal-5.0b1/LICENSE.txt` & `tzlocal-5.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tzlocal-5.0b1/PKG-INFO` & `tzlocal-5.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzlocal
-Version: 5.0b1
+Version: 5.0b2
 Summary: tzinfo object for the local timezone
 Home-page: UNKNOWN
 Author: Lennart Regebro
 Author-email: regebro@gmail.com
 License: MIT
 Project-URL: Source code, https://github.com/regebro/tzlocal
 Project-URL: Issue tracker, https://github.com/regebro/tzlocal/issues
@@ -231,14 +231,27 @@
 -------
 
 * MIT https://opensource.org/licenses/MIT
 
 Changes
 =======
 
+5.0b2 (2023-04-11)
+------------------
+
+- Change how the system offset is calculated to deal with non-DST
+  temporary changes, such as Ramadan time in Morocco.
+
+- Change the default to only warn when the timezone offset and system
+  offset disagree (but still not even warn if TZ is set)
+
+- Add the assert_tz_offset() method to the top level for those who want
+  to explicitly check and fail.
+
+
 5.0b1 (2023-04-07)
 ------------------
 
 - Removed the deprecation shim. 
 
 
 4.4b1 (2023-03-20)
```

### Comparing `tzlocal-5.0b1/README.rst` & `tzlocal-5.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `tzlocal-5.0b1/setup.cfg` & `tzlocal-5.0b2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = tzlocal
 description = tzinfo object for the local timezone
 long_description = file: README.rst, CHANGES.txt
-version = 5.0b1
+version = 5.0b2
 author = Lennart Regebro
 author_email = regebro@gmail.com
 project_urls = 
 	Source code = https://github.com/regebro/tzlocal
 	Issue tracker = https://github.com/regebro/tzlocal/issues
 license = MIT
 keywords = timezone
```

### Comparing `tzlocal-5.0b1/tests/test_tzlocal.py` & `tzlocal-5.0b2/tests/test_tzlocal.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,19 @@
     local = tzlocal.get_localzone()
     tzlocal.utils.assert_tz_offset(local)
 
     # Get a non local zone. Let's use Chatham, population 600.
     other = ZoneInfo("Pacific/Chatham")
     pytest.raises(ValueError, tzlocal.utils.assert_tz_offset, other)
 
+    # But you can change it do it only warns
+    other = ZoneInfo("Pacific/Chatham")
+    with pytest.warns(UserWarning):
+        tzlocal.utils.assert_tz_offset(other, error=False)
+
 
 def test_win32(mocker):
     if sys.platform == "win32":
         # Ironically, these tests don't work on Windows.
         import tzlocal.win32
 
         # Just check on Windows that the code works, and that we get
```

### Comparing `tzlocal-5.0b1/tzlocal/unix.py` & `tzlocal-5.0b2/tzlocal/unix.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             tz = timezone.utc
     else:
         tz = zoneinfo.ZoneInfo(tzname)
 
     if _root == "/":
         # We are using a file in etc to name the timezone.
         # Verify that the timezone specified there is actually used:
-        utils.assert_tz_offset(tz)
+        utils.assert_tz_offset(tz, error=False)
     return tz
 
 
 def get_localzone_name():
     """Get the computers configured local timezone name, if any."""
     global _cache_tz_name
     if _cache_tz_name is None:
```

### Comparing `tzlocal-5.0b1/tzlocal/utils.py` & `tzlocal-5.0b2/tzlocal/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 import logging
 import os
 import time
 import datetime
 import calendar
+import warnings
 
 try:
     import zoneinfo  # pragma: no cover
 except ImportError:
     from backports import zoneinfo  # pragma: no cover
 
 from tzlocal import windows_tz
 
 
-def get_system_offset():
-    """Get system's timezone offset using built-in library time.
-
-    For the Timezone constants (altzone, daylight, timezone, and tzname), the
-    value is determined by the timezone rules in effect at module load time or
-    the last time tzset() is called and may be incorrect for times in the past.
-
-    To keep compatibility with Windows, we're always importing time module here.
-    """
-
-    localtime = calendar.timegm(time.localtime())
-    gmtime = calendar.timegm(time.gmtime())
-    offset = gmtime - localtime
-    # We could get the localtime and gmtime on either side of a second switch
-    # so we check that the difference is less than one minute, because nobody
-    # has that small DST differences.
-    if abs(offset - time.altzone) < 60:
-        return -time.altzone  # pragma: no cover
-    else:
-        return -time.timezone  # pragma: no cover
-
-
 def get_tz_offset(tz):
     """Get timezone's offset using built-in function datetime.utcoffset()."""
     return int(datetime.datetime.now(tz).utcoffset().total_seconds())
 
 
-def assert_tz_offset(tz):
+def assert_tz_offset(tz, error=True):
     """Assert that system's timezone offset equals to the timezone offset found.
 
     If they don't match, we probably have a misconfiguration, for example, an
-    incorrect timezone set in /etc/timezone file in systemd distributions."""
+    incorrect timezone set in /etc/timezone file in systemd distributions.
+
+    If error is True, this method will raise a ValueError, otherwise it will
+    emit a warning.
+    """
+
     tz_offset = get_tz_offset(tz)
-    system_offset = get_system_offset()
-    if tz_offset != system_offset:
+    system_offset = calendar.timegm(time.gmtime()) - calendar.timegm(time.localtime())
+    # No one has timezone offsets less than a minute, so this should be close enough:
+    if abs(tz_offset - system_offset) > 60:
         msg = (
             "Timezone offset does not match system offset: {} != {}. "
             "Please, check your config files."
         ).format(tz_offset, system_offset)
-        raise ValueError(msg)
+        if error:
+            raise ValueError(msg)
+        warnings.warn(msg)
 
 
 def _tz_name_from_env(tzenv=None):
     if tzenv is None:
         tzenv = os.environ.get("TZ")
 
     if not tzenv:
```

### Comparing `tzlocal-5.0b1/tzlocal/win32.py` & `tzlocal-5.0b2/tzlocal/win32.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,20 +126,20 @@
     if _cache_tz is None:
         _cache_tz = zoneinfo.ZoneInfo(get_localzone_name())
 
     if not utils._tz_name_from_env():
         # If the timezone does NOT come from a TZ environment variable,
         # verify that it's correct. If it's from the environment,
         # we accept it, this is so you can run tests with different timezones.
-        utils.assert_tz_offset(_cache_tz)
+        utils.assert_tz_offset(_cache_tz, error=False)
 
     return _cache_tz
 
 
 def reload_localzone():
     """Reload the cached localzone. You need to call this if the timezone has changed."""
     global _cache_tz
     global _cache_tz_name
     _cache_tz_name = _get_localzone_name()
     _cache_tz = zoneinfo.ZoneInfo(_cache_tz_name)
-    utils.assert_tz_offset(_cache_tz)
+    utils.assert_tz_offset(_cache_tz, error=False)
     return _cache_tz
```

### Comparing `tzlocal-5.0b1/tzlocal/windows_tz.py` & `tzlocal-5.0b2/tzlocal/windows_tz.py`

 * *Files identical despite different names*

### Comparing `tzlocal-5.0b1/tzlocal.egg-info/PKG-INFO` & `tzlocal-5.0b2/tzlocal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzlocal
-Version: 5.0b1
+Version: 5.0b2
 Summary: tzinfo object for the local timezone
 Home-page: UNKNOWN
 Author: Lennart Regebro
 Author-email: regebro@gmail.com
 License: MIT
 Project-URL: Source code, https://github.com/regebro/tzlocal
 Project-URL: Issue tracker, https://github.com/regebro/tzlocal/issues
@@ -231,14 +231,27 @@
 -------
 
 * MIT https://opensource.org/licenses/MIT
 
 Changes
 =======
 
+5.0b2 (2023-04-11)
+------------------
+
+- Change how the system offset is calculated to deal with non-DST
+  temporary changes, such as Ramadan time in Morocco.
+
+- Change the default to only warn when the timezone offset and system
+  offset disagree (but still not even warn if TZ is set)
+
+- Add the assert_tz_offset() method to the top level for those who want
+  to explicitly check and fail.
+
+
 5.0b1 (2023-04-07)
 ------------------
 
 - Removed the deprecation shim. 
 
 
 4.4b1 (2023-03-20)
```

### Comparing `tzlocal-5.0b1/tzlocal.egg-info/SOURCES.txt` & `tzlocal-5.0b2/tzlocal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tzlocal-5.0b1/update_windows_mappings.py` & `tzlocal-5.0b2/update_windows_mappings.py`

 * *Files identical despite different names*

