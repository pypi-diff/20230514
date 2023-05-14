# Comparing `tmp/pyphysio-3.1.4.tar.gz` & `tmp/pyphysio-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphysio-3.1.4.tar", last modified: Thu Apr 20 13:17:17 2023, max compression
+gzip compressed data, was "pyphysio-3.1.5.tar", last modified: Sun May 14 13:53:04 2023, max compression
```

## Comparing `pyphysio-3.1.4.tar` & `pyphysio-3.1.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.674972 pyphysio-3.1.4/
--rwx------   0 bizzego   (1002) bizzego   (1002)    35142 2019-02-28 14:12:28.000000 pyphysio-3.1.4/LICENSE
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)      879 2023-04-20 13:17:17.674972 pyphysio-3.1.4/PKG-INFO
--rwx------   0 bizzego   (1002) bizzego   (1002)      730 2023-03-24 15:13:33.000000 pyphysio-3.1.4/README.md
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.590971 pyphysio-3.1.4/pyphysio/
--rwx------   0 bizzego   (1002) bizzego   (1002)     1468 2023-03-27 13:38:27.000000 pyphysio-3.1.4/pyphysio/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    12620 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/_base_algorithm.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    13300 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/artefacts.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    22321 2023-04-05 14:15:39.000000 pyphysio-3.1.4/pyphysio/filters.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio/generators/
--rwx------   0 bizzego   (1002) bizzego   (1002)     3714 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/generators/__init__.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio/indicators/
--rwx------   0 bizzego   (1002) bizzego   (1002)      374 2023-04-05 14:15:39.000000 pyphysio-3.1.4/pyphysio/indicators/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     2676 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/indicators/frequencydomain.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    11155 2023-04-05 14:15:40.000000 pyphysio-3.1.4/pyphysio/indicators/nonlinear.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    17343 2023-04-17 09:46:09.000000 pyphysio-3.1.4/pyphysio/indicators/peaks.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     6892 2023-04-05 14:15:40.000000 pyphysio-3.1.4/pyphysio/indicators/timedomain.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     9305 2023-04-20 13:09:16.000000 pyphysio-3.1.4/pyphysio/interactive.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio/loaders/
--rwx------   0 bizzego   (1002) bizzego   (1002)      108 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/loaders/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    18226 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/loaders/_load_nirx.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    13169 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/segmenters.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    17232 2023-04-06 12:32:55.000000 pyphysio-3.1.4/pyphysio/signal.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.558970 pyphysio-3.1.4/pyphysio/specialized/
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio/specialized/activity/
--rwx------   0 bizzego   (1002) bizzego   (1002)      632 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/activity/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/eda/
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     6887 2023-04-13 12:45:40.000000 pyphysio-3.1.4/pyphysio/specialized/eda/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1026 2023-03-27 13:38:27.000000 pyphysio-3.1.4/pyphysio/specialized/eda/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/eeg/
--rwx------   0 bizzego   (1002) bizzego   (1002)      768 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/eeg/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/emg/
--rwx------   0 bizzego   (1002) bizzego   (1002)      628 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/emg/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/fnirs/
--rwx------   0 bizzego   (1002) bizzego   (1002)     9787 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/fnirs/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    10447 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/fnirs/_convert.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    24210 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/fnirs/_data.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     2718 2023-03-24 10:35:17.000000 pyphysio-3.1.4/pyphysio/specialized/fnirs/_dl_sqi.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/heart/
--rwx------   0 bizzego   (1002) bizzego   (1002)    27262 2023-04-19 14:25:16.000000 pyphysio-3.1.4/pyphysio/specialized/heart/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1957 2023-04-05 14:15:40.000000 pyphysio-3.1.4/pyphysio/specialized/heart/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.598971 pyphysio-3.1.4/pyphysio/specialized/resp/
--rwx------   0 bizzego   (1002) bizzego   (1002)      630 2023-03-24 10:35:18.000000 pyphysio-3.1.4/pyphysio/specialized/resp/_presets.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     6272 2023-03-24 10:35:18.000000 pyphysio-3.1.4/pyphysio/sqi.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.618971 pyphysio-3.1.4/pyphysio/test_data/
--rwx------   0 bizzego   (1002) bizzego   (1002)       64 2023-03-27 13:38:27.000000 pyphysio-3.1.4/pyphysio/test_data/info_medical
--rwx------   0 bizzego   (1002) bizzego   (1002)  1097515 2023-03-27 13:38:27.000000 pyphysio-3.1.4/pyphysio/test_data/medical.txt.bz2
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    34172 2023-04-13 12:44:09.000000 pyphysio-3.1.4/pyphysio/utils.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.594971 pyphysio-3.1.4/pyphysio.egg-info/
--rwx------   0 bizzego   (1002) bizzego   (1002)      879 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/PKG-INFO
--rwx------   0 bizzego   (1002) bizzego   (1002)     1355 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/SOURCES.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)        1 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/dependency_links.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)       54 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/requires.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)        9 2023-04-20 13:17:17.000000 pyphysio-3.1.4/pyphysio.egg-info/top_level.txt
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)       38 2023-04-20 13:17:17.674972 pyphysio-3.1.4/setup.cfg
--rwx------   0 bizzego   (1002) bizzego   (1002)     2290 2023-04-20 13:16:46.000000 pyphysio-3.1.4/setup.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-04-20 13:17:17.674972 pyphysio-3.1.4/tests/
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8337 2023-04-13 12:55:10.000000 pyphysio-3.1.4/tests/test_eda_methods.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1201 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_filters.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1581 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_fnirs.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      547 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_get_sampling_freq.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      600 2023-04-19 07:37:36.000000 pyphysio-3.1.4/tests/test_ibi_estimators.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1016 2023-03-24 10:35:18.000000 pyphysio-3.1.4/tests/test_segmenters.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      959 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_signal.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     4535 2023-03-27 13:38:27.000000 pyphysio-3.1.4/tests/test_tools.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.209657 pyphysio-3.1.5/
+-rwx------   0 bizzego   (1002) bizzego   (1002)    35142 2019-02-28 14:12:28.000000 pyphysio-3.1.5/LICENSE
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)      879 2023-05-14 13:53:04.209657 pyphysio-3.1.5/PKG-INFO
+-rwx------   0 bizzego   (1002) bizzego   (1002)      730 2023-03-24 15:13:33.000000 pyphysio-3.1.5/README.md
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.181656 pyphysio-3.1.5/pyphysio/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1468 2023-03-27 13:38:27.000000 pyphysio-3.1.5/pyphysio/__init__.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    12606 2023-05-08 08:55:48.000000 pyphysio-3.1.5/pyphysio/_base_algorithm.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    13300 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/artefacts.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    22321 2023-04-05 14:15:39.000000 pyphysio-3.1.5/pyphysio/filters.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.181656 pyphysio-3.1.5/pyphysio/generators/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     3714 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/generators/__init__.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/indicators/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      374 2023-04-05 14:15:39.000000 pyphysio-3.1.5/pyphysio/indicators/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2676 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/indicators/frequencydomain.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    11155 2023-04-05 14:15:40.000000 pyphysio-3.1.5/pyphysio/indicators/nonlinear.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    17343 2023-04-17 09:46:09.000000 pyphysio-3.1.5/pyphysio/indicators/peaks.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     6892 2023-04-05 14:15:40.000000 pyphysio-3.1.5/pyphysio/indicators/timedomain.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     9305 2023-04-20 13:09:16.000000 pyphysio-3.1.5/pyphysio/interactive.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/loaders/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      108 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/loaders/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    18226 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/loaders/_load_nirx.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    13284 2023-05-08 07:37:50.000000 pyphysio-3.1.5/pyphysio/segmenters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    17232 2023-04-06 12:32:55.000000 pyphysio-3.1.5/pyphysio/signal.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.149657 pyphysio-3.1.5/pyphysio/specialized/
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/specialized/activity/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      632 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/specialized/activity/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/specialized/eda/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     7011 2023-05-14 13:50:04.000000 pyphysio-3.1.5/pyphysio/specialized/eda/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1026 2023-03-27 13:38:27.000000 pyphysio-3.1.5/pyphysio/specialized/eda/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/specialized/eeg/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      768 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/specialized/eeg/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/specialized/emg/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      628 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/specialized/emg/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/specialized/fnirs/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     9787 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/specialized/fnirs/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    10447 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/specialized/fnirs/_convert.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    24210 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/specialized/fnirs/_data.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2718 2023-03-24 10:35:17.000000 pyphysio-3.1.5/pyphysio/specialized/fnirs/_dl_sqi.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/specialized/heart/
+-rwx------   0 bizzego   (1002) bizzego   (1002)    27262 2023-04-19 14:25:16.000000 pyphysio-3.1.5/pyphysio/specialized/heart/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1957 2023-04-05 14:15:40.000000 pyphysio-3.1.5/pyphysio/specialized/heart/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.185656 pyphysio-3.1.5/pyphysio/specialized/resp/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      630 2023-03-24 10:35:18.000000 pyphysio-3.1.5/pyphysio/specialized/resp/_presets.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     6272 2023-03-24 10:35:18.000000 pyphysio-3.1.5/pyphysio/sqi.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.205657 pyphysio-3.1.5/pyphysio/test_data/
+-rwx------   0 bizzego   (1002) bizzego   (1002)       64 2023-03-27 13:38:27.000000 pyphysio-3.1.5/pyphysio/test_data/info_medical
+-rwx------   0 bizzego   (1002) bizzego   (1002)  1097515 2023-03-27 13:38:27.000000 pyphysio-3.1.5/pyphysio/test_data/medical.txt.bz2
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    34067 2023-05-14 13:42:50.000000 pyphysio-3.1.5/pyphysio/utils.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.181656 pyphysio-3.1.5/pyphysio.egg-info/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      879 2023-05-14 13:53:04.000000 pyphysio-3.1.5/pyphysio.egg-info/PKG-INFO
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1355 2023-05-14 13:53:04.000000 pyphysio-3.1.5/pyphysio.egg-info/SOURCES.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)        1 2023-05-14 13:53:04.000000 pyphysio-3.1.5/pyphysio.egg-info/dependency_links.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)       54 2023-05-14 13:53:04.000000 pyphysio-3.1.5/pyphysio.egg-info/requires.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)        9 2023-05-14 13:53:04.000000 pyphysio-3.1.5/pyphysio.egg-info/top_level.txt
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)       38 2023-05-14 13:53:04.209657 pyphysio-3.1.5/setup.cfg
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2290 2023-05-14 13:52:44.000000 pyphysio-3.1.5/setup.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-05-14 13:53:04.209657 pyphysio-3.1.5/tests/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8596 2023-05-14 13:47:52.000000 pyphysio-3.1.5/tests/test_eda_methods.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1201 2023-03-27 13:38:27.000000 pyphysio-3.1.5/tests/test_filters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1581 2023-03-27 13:38:27.000000 pyphysio-3.1.5/tests/test_fnirs.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      547 2023-03-27 13:38:27.000000 pyphysio-3.1.5/tests/test_get_sampling_freq.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      600 2023-04-19 07:37:36.000000 pyphysio-3.1.5/tests/test_ibi_estimators.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1016 2023-03-24 10:35:18.000000 pyphysio-3.1.5/tests/test_segmenters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      959 2023-03-27 13:38:27.000000 pyphysio-3.1.5/tests/test_signal.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     4535 2023-03-27 13:38:27.000000 pyphysio-3.1.5/tests/test_tools.py
```

### Comparing `pyphysio-3.1.4/LICENSE` & `pyphysio-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/PKG-INFO` & `pyphysio-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphysio
-Version: 3.1.4
+Version: 3.1.5
 Summary: Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)
 Home-page: https://gitlab.com/a.bizzego/pyphysio
 Author: a.bizzego
 Author-email: andrea.bizzego@unitn.it
 Keywords: eda,gsr,ecg,bvp,fnirs,signal,analysis,physiological,psychopysiology,neuroscience
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
```

### Comparing `pyphysio-3.1.4/README.md` & `pyphysio-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/__init__.py` & `pyphysio-3.1.5/pyphysio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/_base_algorithm.py` & `pyphysio-3.1.5/pyphysio/_base_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
                                       template = template_dask)
             #apply the rollink mechanism and compose the results
             signal_out = mapper.load(scheduler=scheduler) #distributed, single-threaded
 
         #The user will mainly call Algorithms on a Dataset
         #so it will expect a Dataset as result
         if isinstance(signal_in, _xr.Dataset):
-            output_name = f'{signal_name}_{self.name}'
+            output_name = f'{signal_name}_{self.__repr__()}'
 
             #TODO: why are we repeating these? they are also in __mapper_func__?
             # we should decide what happens to a dataset when an algorithm is applied!!!
             # we could just transform to _xr.Dataset?
             
             #add windowing info
             strange_result = False
@@ -288,15 +288,15 @@
             else:
                 signal_out = signal_out.assign_coords({dim:_np.arange(signal_out.sizes[dim])})
                     
         signal_out.attrs = signal_in.attrs.copy()
         return(signal_out)
     
     def __repr__(self):
-        return self.__class__.__name__ + str(self._params) if 'name' not in self._params else self._params['name']
+        return self.__class__.__name__ if 'name' not in self._params else self._params['name']
 
     def set_params(self, **kwargs):
         self._params.update(kwargs)
 
     def set(self, **kwargs):
         kk = self.get()
         kk.update(kwargs)
```

### Comparing `pyphysio-3.1.4/pyphysio/artefacts.py` & `pyphysio-3.1.5/pyphysio/artefacts.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/filters.py` & `pyphysio-3.1.5/pyphysio/filters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/generators/__init__.py` & `pyphysio-3.1.5/pyphysio/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/indicators/frequencydomain.py` & `pyphysio-3.1.5/pyphysio/indicators/frequencydomain.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/indicators/nonlinear.py` & `pyphysio-3.1.5/pyphysio/indicators/nonlinear.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/indicators/peaks.py` & `pyphysio-3.1.5/pyphysio/indicators/peaks.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/indicators/timedomain.py` & `pyphysio-3.1.5/pyphysio/indicators/timedomain.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/interactive.py` & `pyphysio-3.1.5/pyphysio/interactive.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/loaders/_load_nirx.py` & `pyphysio-3.1.5/pyphysio/loaders/_load_nirx.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/segmenters.py` & `pyphysio-3.1.5/pyphysio/segmenters.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,26 +323,27 @@
     #for all algorithms
     for alg in algorithms:
         # print(alg.name)
         result_algorithm = []
         for i_seg, seg in enumerate(segmenter): #this generates segments from the segmenter
             # print(seg.get_begin_time())    
             signal_segment = seg(signal)
-            res = alg(signal_segment, add_signal=True)
-            res = res.drop(signal_name)
-            res = res.dropna(dim='time', 
-                             how='all', 
-                             subset=[f'{signal_name}_{alg.name}'])
-            res = res.assign_coords(label=('time', [seg.get_label()]))
-            
-            result_algorithm.append(res)
+            if signal_segment.p.get_values().shape[0] > 0:
+                res = alg(signal_segment, add_signal=True)
+                res = res.drop(signal_name)
+                res = res.dropna(dim='time', 
+                                 how='all', 
+                                 subset=[f'{signal_name}_{alg.__repr__()}'])
+                res = res.assign_coords(label=('time', [seg.get_label()]))
+                
+                result_algorithm.append(res)
 
         result.append(_xr.concat(result_algorithm, dim='time'))
 
-    result = _xr.merge(result)
+    result = _xr.merge(result,compat='override')
     return result
 
 #TODO: needed? if yes, fix--->
 '''
 def indicators2df(fmap_results):
     import pandas as _pd
```

### Comparing `pyphysio-3.1.4/pyphysio/signal.py` & `pyphysio-3.1.5/pyphysio/signal.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/activity/_presets.py` & `pyphysio-3.1.5/pyphysio/specialized/activity/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/eda/__init__.py` & `pyphysio-3.1.5/pyphysio/specialized/eda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,35 +137,37 @@
         # grid_size = params["grid_size"]
         win_pre = params['win_pre']
         win_post = params['win_post']
         return_phasic = params['return_phasic']
 
         fsamp = signal.p.get_sampling_freq()
         signal_values = signal.p.get_values().ravel()
-
+        
         # find peaks in the driver
         maxima = _PeakDetection(delta=amplitude, refractory=1, start_max=True, return_peaks=True)(signal)
-        maxp = _np.where(~_np.isnan(maxima.p.main_signal.values))[0].ravel()
-
-        # identify start and stop of the peaks
-        peaks = _PeakSelection(indices=maxp, win_pre=win_pre, win_post=win_post)(signal)
+        idx_maxp = _np.where(~_np.isnan(maxima.p.main_signal.values))[0].ravel()
+        # print(idx_maxp)
         
+        # identify start and stop of the peaks
+        peaks = _PeakSelection(indices=idx_maxp, win_pre=win_pre, win_post=win_post)(signal)
+        # print(peaks.p.get_values().ravel())
         # find tonic component (= portion outside the peaks ==> peaks == 0)
         idx_tonic = _np.where(peaks.p.get_values().ravel() == 0)[0]
         
         #first and last sample should be included
         if idx_tonic[0] != 0:
             idx_tonic = _np.insert(idx_tonic, 0, 0)
         
         if idx_tonic[-1] != (len(signal_values) - 1):
             idx_tonic = _np.insert(idx_tonic, len(idx_tonic), len(signal_values) - 1)
         
+        
         tonic_interp = signal_values[idx_tonic]
 
-        tonic = create_signal(tonic_interp, times = idx_tonic/fsamp)
+        tonic = create_signal(tonic_interp, times = idx_tonic/fsamp + signal.p.get_start_time())
         tonic = tonic.interp({'time': signal.p.get_times()}, 'cubic')
         tonic_values = tonic.p.get_values().ravel()
         
         # fitter = _np.poly1d(_np.polyfit(idx_tonic, driver_interp, 10))
         # tonic = fitter(_np.arange(len(signal_values)))
 
         if not return_phasic:
```

### Comparing `pyphysio-3.1.4/pyphysio/specialized/eda/_presets.py` & `pyphysio-3.1.5/pyphysio/specialized/eda/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/eeg/_presets.py` & `pyphysio-3.1.5/pyphysio/specialized/eeg/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/emg/_presets.py` & `pyphysio-3.1.5/pyphysio/specialized/emg/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/fnirs/__init__.py` & `pyphysio-3.1.5/pyphysio/specialized/fnirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/fnirs/_convert.py` & `pyphysio-3.1.5/pyphysio/specialized/fnirs/_convert.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/fnirs/_data.py` & `pyphysio-3.1.5/pyphysio/specialized/fnirs/_data.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/fnirs/_dl_sqi.py` & `pyphysio-3.1.5/pyphysio/specialized/fnirs/_dl_sqi.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/heart/__init__.py` & `pyphysio-3.1.5/pyphysio/specialized/heart/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/heart/_presets.py` & `pyphysio-3.1.5/pyphysio/specialized/heart/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/specialized/resp/_presets.py` & `pyphysio-3.1.5/pyphysio/specialized/resp/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/sqi.py` & `pyphysio-3.1.5/pyphysio/sqi.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/test_data/medical.txt.bz2` & `pyphysio-3.1.5/pyphysio/test_data/medical.txt.bz2`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/pyphysio/utils.py` & `pyphysio-3.1.5/pyphysio/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,34 +907,30 @@
         
         params = self._params
         i_peaks = params['indices']
         i_pre_max = int(params['win_pre'] * signal.p.get_sampling_freq())
         i_post_max = int(params['win_post'] * signal.p.get_sampling_freq())
         
         signal_values = signal.p.get_values().ravel()
-        
         dd = _np.convolve(_np.diff(signal_values)//1.0, _np.ones(2)/2)
+
         i_start = []
         i_stop = []
 
         
         for idx_max in i_peaks:
+
             idx_pre = idx_max-1
-            s_pre = dd[idx_pre]
-            while ((s_pre>-0.5) and ((idx_max-idx_pre) <= i_pre_max)):
+            while ((dd[idx_pre]>-0.5) and ((idx_max-idx_pre) <= i_pre_max)) and (idx_pre>0):
                 idx_pre -=1
-                s_pre = dd[idx_pre]
-            idx_pre +=1
             i_start.append(idx_pre)
             
             idx_post = idx_max+1
-            s_post = dd[idx_post]
-            while ((s_post<-0.5) and ((idx_post-idx_max) <= i_post_max)):
+            while ((dd[idx_post]<-0.5) and ((idx_post-idx_max) <= i_post_max)) and (idx_post<(len(signal_values)-1)):
                 idx_post +=1
-                s_post = dd[idx_post]
             idx_post -=1    
             i_stop.append(idx_post)
         
         
         
         
         # i_start = _np.empty(len(i_peaks), int)
```

### Comparing `pyphysio-3.1.4/pyphysio.egg-info/PKG-INFO` & `pyphysio-3.1.5/pyphysio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphysio
-Version: 3.1.4
+Version: 3.1.5
 Summary: Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)
 Home-page: https://gitlab.com/a.bizzego/pyphysio
 Author: a.bizzego
 Author-email: andrea.bizzego@unitn.it
 Keywords: eda,gsr,ecg,bvp,fnirs,signal,analysis,physiological,psychopysiology,neuroscience
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
```

### Comparing `pyphysio-3.1.4/pyphysio.egg-info/SOURCES.txt` & `pyphysio-3.1.5/pyphysio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/setup.py` & `pyphysio-3.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
               'pyphysio.specialized.fnirs',
               'pyphysio.specialized.heart',
               'pyphysio.specialized.resp',
               'pyphysio.indicators',
               'pyphysio.generators'],
     package_data={'pyphysio': ['test_data/*']},
     # data_files={'test_data_out': ['info_medical', 'medical.txt.bz2']},
-    version='3.1.4',
+    version='3.1.5',
     description='Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)',
     author='a.bizzego',
     author_email='andrea.bizzego@unitn.it',
     url='https://gitlab.com/a.bizzego/pyphysio',
     keywords=['eda', 'gsr', 'ecg', 'bvp', 'fnirs', 'signal', 
               'analysis', 'physiological', 'psychopysiology', 'neuroscience'],
     classifiers=[
```

### Comparing `pyphysio-3.1.4/tests/test_eda_methods.py` & `pyphysio-3.1.5/tests/test_eda_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,36 @@
 signal = create_signal(eda_data, sampling_freq=2048)
 
 #%%
 # signal = ph.load('/home/bizzego/UniTn/didattica/neurotechnology/datasets/DEAP/signals/eda/s21')
 signal = flt.ConvolutionalFilter('rect', 2)(signal)
 
 # signal /=1000
+#%%
+# signal = ph.load('/home/bizzego/Downloads/recognitiveneuroscienceandneurotechnology/P2_Base1')
 
 #%%
+# signal = flt.ConvolutionalFilter('rect', 1, normalize=True)(signal)
 fsamp = 8
 signal = signal.p.resample(fsamp)
 driver = eda_tools.DriverEstim(t1=0.25, t2=10)(signal)
 
 driver = flt.ConvolutionalFilter('rect', 1, normalize=True)(driver)
-
 # driver.p.plot()
+
 # driver_.p.plot()
 
-phasic = eda_tools.PhasicEstim(0.005, win_pre=3, win_post=3)(driver)
-tonic = eda_tools.PhasicEstim(0.005, win_pre=3, win_post=3, return_phasic=False)(driver)
+#%%
+# driver.p.segment_time(5, 7).p.plot('.')
+phasic = eda_tools.PhasicEstim(1, win_pre=3, win_post=3)(driver)#.p.segment_time(5, 7))
+
+# phasic.p.plot('.')
+
+#%%
+tonic = eda_tools.PhasicEstim(1, win_pre=3, win_post=3, return_phasic=False)(driver)
 
 #%%
 # driver.p.plot()
 # tonic.p.plot()
 # phasic.p.plot()
 # plt.show()
```

### Comparing `pyphysio-3.1.4/tests/test_filters.py` & `pyphysio-3.1.5/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/tests/test_fnirs.py` & `pyphysio-3.1.5/tests/test_fnirs.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/tests/test_get_sampling_freq.py` & `pyphysio-3.1.5/tests/test_get_sampling_freq.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/tests/test_ibi_estimators.py` & `pyphysio-3.1.5/tests/test_ibi_estimators.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/tests/test_segmenters.py` & `pyphysio-3.1.5/tests/test_segmenters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/tests/test_signal.py` & `pyphysio-3.1.5/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.4/tests/test_tools.py` & `pyphysio-3.1.5/tests/test_tools.py`

 * *Files identical despite different names*

