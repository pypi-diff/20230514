# Comparing `tmp/pypinyin-dict-0.5.0.tar.gz` & `tmp/pypinyin-dict-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypinyin-dict-0.5.0.tar", last modified: Sun Jan 15 07:30:54 2023, max compression
+gzip compressed data, was "pypinyin-dict-0.6.0.tar", last modified: Sun May 14 12:34:07 2023, max compression
```

## Comparing `pypinyin-dict-0.5.0.tar` & `pypinyin-dict-0.6.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-01-15 07:30:54.514814 pypinyin-dict-0.5.0/
--rw-r--r--   0 mg         (501) wheel        (0)     4482 2023-01-15 07:30:54.515023 pypinyin-dict-0.5.0/PKG-INFO
--rw-r--r--   0 mg         (501) wheel        (0)     2821 2022-11-06 02:35:11.000000 pypinyin-dict-0.5.0/README.md
--rw-r--r--   0 mg         (501) wheel        (0)      105 2021-09-20 04:13:18.000000 pypinyin-dict-0.5.0/pyproject.toml
--rw-r--r--   0 mg         (501) wheel        (0)       67 2023-01-15 07:30:54.515555 pypinyin-dict-0.5.0/setup.cfg
--rw-r--r--   0 mg         (501) wheel        (0)     1122 2023-01-15 07:24:20.000000 pypinyin-dict-0.5.0/setup.py
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-01-15 07:30:54.327874 pypinyin-dict-0.5.0/src/
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-01-15 07:30:54.329687 pypinyin-dict-0.5.0/src/pypinyin_dict/
--rw-r--r--   0 mg         (501) wheel        (0)       24 2021-09-19 13:37:01.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/__init__.py
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-01-15 07:30:54.494800 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/
--rw-r--r--   0 mg         (501) wheel        (0)       24 2021-09-19 13:37:01.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/__init__.py
--rw-r--r--   0 mg         (501) wheel        (0)      634 2023-01-15 07:21:35.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict.py
--rw-r--r--   0 mg         (501) wheel        (0)  1681130 2023-01-15 07:21:35.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_0.py
--rw-r--r--   0 mg         (501) wheel        (0)  1617555 2023-01-15 07:21:35.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_1.py
--rw-r--r--   0 mg         (501) wheel        (0)  1614814 2023-01-15 07:21:35.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_2.py
--rw-r--r--   0 mg         (501) wheel        (0)      275 2023-01-15 07:21:35.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_3.py
--rw-r--r--   0 mg         (501) wheel        (0)   392409 2023-01-15 07:21:35.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/di.py
--rw-r--r--   0 mg         (501) wheel        (0)     1430 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin.py
--rw-r--r--   0 mg         (501) wheel        (0)  1860938 2023-01-15 07:21:37.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_0.py
--rw-r--r--   0 mg         (501) wheel        (0)  1794721 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_1.py
--rw-r--r--   0 mg         (501) wheel        (0)      347 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_10.py
--rw-r--r--   0 mg         (501) wheel        (0)  1762509 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_2.py
--rw-r--r--   0 mg         (501) wheel        (0)  1738446 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_3.py
--rw-r--r--   0 mg         (501) wheel        (0)  1774086 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_4.py
--rw-r--r--   0 mg         (501) wheel        (0)  1756773 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_5.py
--rw-r--r--   0 mg         (501) wheel        (0)  1735094 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_6.py
--rw-r--r--   0 mg         (501) wheel        (0)  1726494 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_7.py
--rw-r--r--   0 mg         (501) wheel        (0)  1696137 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_8.py
--rw-r--r--   0 mg         (501) wheel        (0)  1741684 2023-01-15 07:21:38.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_9.py
--rw-r--r--   0 mg         (501) wheel        (0)  2350525 2023-01-15 07:21:29.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/pinyin.py
--rw-r--r--   0 mg         (501) wheel        (0)     1050 2023-01-15 07:21:33.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs.py
--rw-r--r--   0 mg         (501) wheel        (0)  1863252 2023-01-15 07:21:32.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_0.py
--rw-r--r--   0 mg         (501) wheel        (0)  1804764 2023-01-15 07:21:32.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_1.py
--rw-r--r--   0 mg         (501) wheel        (0)  1761345 2023-01-15 07:21:32.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_2.py
--rw-r--r--   0 mg         (501) wheel        (0)  1793548 2023-01-15 07:21:33.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_3.py
--rw-r--r--   0 mg         (501) wheel        (0)  1788871 2023-01-15 07:21:33.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_4.py
--rw-r--r--   0 mg         (501) wheel        (0)  1761721 2023-01-15 07:21:33.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_5.py
--rw-r--r--   0 mg         (501) wheel        (0)  1734876 2023-01-15 07:21:33.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_6.py
--rw-r--r--   0 mg         (501) wheel        (0)  1788828 2023-01-15 07:21:33.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_7.py
--rw-r--r--   0 mg         (501) wheel        (0)      634 2023-01-15 07:21:34.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs.py
--rw-r--r--   0 mg         (501) wheel        (0)   681449 2023-01-15 07:21:34.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_0.py
--rw-r--r--   0 mg         (501) wheel        (0)   681855 2023-01-15 07:21:34.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_1.py
--rw-r--r--   0 mg         (501) wheel        (0)   680792 2023-01-15 07:21:34.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_2.py
--rw-r--r--   0 mg         (501) wheel        (0)      283 2023-01-15 07:21:34.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_3.py
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-01-15 07:30:54.512160 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/
--rw-r--r--   0 mg         (501) wheel        (0)       24 2021-09-19 13:37:01.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/__init__.py
--rw-r--r--   0 mg         (501) wheel        (0)   131893 2023-01-15 07:21:28.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/cc_cedict.py
--rw-r--r--   0 mg         (501) wheel        (0)    79137 2023-01-15 07:21:28.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/khanyupinlu.py
--rw-r--r--   0 mg         (501) wheel        (0)   752878 2023-01-15 07:21:28.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/khanyupinyin.py
--rw-r--r--   0 mg         (501) wheel        (0)   163153 2023-01-15 07:21:28.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/kmandarin_8105.py
--rw-r--r--   0 mg         (501) wheel        (0)   166528 2023-01-15 07:21:28.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/ktghz2013.py
--rw-r--r--   0 mg         (501) wheel        (0)   228831 2023-01-15 07:21:28.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/kxhc1983.py
--rw-r--r--   0 mg         (501) wheel        (0)   905695 2023-01-15 07:21:28.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/pinyin.py
--rw-r--r--   0 mg         (501) wheel        (0)   896193 2023-01-15 07:21:28.000000 pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/zdic.py
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-01-15 07:30:54.331541 pypinyin-dict-0.5.0/src/pypinyin_dict.egg-info/
--rw-r--r--   0 mg         (501) wheel        (0)     4482 2023-01-15 07:30:53.000000 pypinyin-dict-0.5.0/src/pypinyin_dict.egg-info/PKG-INFO
--rw-r--r--   0 mg         (501) wheel        (0)     2444 2023-01-15 07:30:53.000000 pypinyin-dict-0.5.0/src/pypinyin_dict.egg-info/SOURCES.txt
--rw-r--r--   0 mg         (501) wheel        (0)        1 2023-01-15 07:30:53.000000 pypinyin-dict-0.5.0/src/pypinyin_dict.egg-info/dependency_links.txt
--rw-r--r--   0 mg         (501) wheel        (0)        9 2023-01-15 07:30:53.000000 pypinyin-dict-0.5.0/src/pypinyin_dict.egg-info/requires.txt
--rw-r--r--   0 mg         (501) wheel        (0)       14 2023-01-15 07:30:53.000000 pypinyin-dict-0.5.0/src/pypinyin_dict.egg-info/top_level.txt
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-05-14 12:34:07.173956 pypinyin-dict-0.6.0/
+-rw-r--r--   0 mg         (501) wheel        (0)     4482 2023-05-14 12:34:07.174175 pypinyin-dict-0.6.0/PKG-INFO
+-rw-r--r--   0 mg         (501) wheel        (0)     2821 2023-01-15 07:32:56.000000 pypinyin-dict-0.6.0/README.md
+-rw-r--r--   0 mg         (501) wheel        (0)      105 2021-09-20 04:13:18.000000 pypinyin-dict-0.6.0/pyproject.toml
+-rw-r--r--   0 mg         (501) wheel        (0)       67 2023-05-14 12:34:07.174845 pypinyin-dict-0.6.0/setup.cfg
+-rw-r--r--   0 mg         (501) wheel        (0)     1122 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/setup.py
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-05-14 12:34:06.928493 pypinyin-dict-0.6.0/src/
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-05-14 12:34:06.930550 pypinyin-dict-0.6.0/src/pypinyin_dict/
+-rw-r--r--   0 mg         (501) wheel        (0)       24 2021-09-19 13:37:01.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/__init__.py
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-05-14 12:34:07.149441 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/
+-rw-r--r--   0 mg         (501) wheel        (0)       24 2021-09-19 13:37:01.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/__init__.py
+-rw-r--r--   0 mg         (501) wheel        (0)      634 2023-05-14 12:25:59.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1681130 2023-05-14 12:25:59.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_0.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1617555 2023-05-14 12:25:59.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_1.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1614814 2023-05-14 12:25:59.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_2.py
+-rw-r--r--   0 mg         (501) wheel        (0)      275 2023-05-14 12:25:59.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_3.py
+-rw-r--r--   0 mg         (501) wheel        (0)   392409 2023-05-14 12:25:59.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/di.py
+-rw-r--r--   0 mg         (501) wheel        (0)     1430 2023-05-14 12:26:02.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1860963 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_0.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1794721 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_1.py
+-rw-r--r--   0 mg         (501) wheel        (0)      382 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_10.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1762509 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_2.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1738421 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_3.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1774113 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_4.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1756708 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_5.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1735157 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_6.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1726495 2023-05-14 12:27:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_7.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1696137 2023-05-14 12:27:55.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_8.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1741685 2023-05-14 12:27:55.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_9.py
+-rw-r--r--   0 mg         (501) wheel        (0)  2350659 2023-05-14 12:27:55.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/pinyin.py
+-rw-r--r--   0 mg         (501) wheel        (0)     1050 2023-05-14 12:25:58.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1863252 2023-05-14 12:25:57.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_0.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1804764 2023-05-14 12:25:57.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_1.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1761345 2023-05-14 12:25:57.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_2.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1793548 2023-05-14 12:25:57.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_3.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1788871 2023-05-14 12:25:57.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_4.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1761721 2023-05-14 12:25:57.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_5.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1734876 2023-05-14 12:27:55.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_6.py
+-rw-r--r--   0 mg         (501) wheel        (0)  1788828 2023-05-14 12:25:58.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_7.py
+-rw-r--r--   0 mg         (501) wheel        (0)      634 2023-05-14 12:25:58.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs.py
+-rw-r--r--   0 mg         (501) wheel        (0)   681449 2023-05-14 12:25:58.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_0.py
+-rw-r--r--   0 mg         (501) wheel        (0)   681855 2023-05-14 12:25:58.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_1.py
+-rw-r--r--   0 mg         (501) wheel        (0)   680792 2023-05-14 12:27:55.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_2.py
+-rw-r--r--   0 mg         (501) wheel        (0)      283 2023-05-14 12:25:58.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_3.py
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-05-14 12:34:07.170570 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/
+-rw-r--r--   0 mg         (501) wheel        (0)       24 2021-09-19 13:37:01.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/__init__.py
+-rw-r--r--   0 mg         (501) wheel        (0)   131893 2023-05-14 12:25:55.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/cc_cedict.py
+-rw-r--r--   0 mg         (501) wheel        (0)    79137 2023-05-14 12:25:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/khanyupinlu.py
+-rw-r--r--   0 mg         (501) wheel        (0)   752878 2023-05-14 12:25:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/khanyupinyin.py
+-rw-r--r--   0 mg         (501) wheel        (0)   163153 2023-05-14 12:25:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/kmandarin_8105.py
+-rw-r--r--   0 mg         (501) wheel        (0)   166528 2023-05-14 12:25:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/ktghz2013.py
+-rw-r--r--   0 mg         (501) wheel        (0)   228831 2023-05-14 12:25:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/kxhc1983.py
+-rw-r--r--   0 mg         (501) wheel        (0)   905695 2023-05-14 12:25:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/pinyin.py
+-rw-r--r--   0 mg         (501) wheel        (0)   896193 2023-05-14 12:25:54.000000 pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/zdic.py
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-05-14 12:34:06.933321 pypinyin-dict-0.6.0/src/pypinyin_dict.egg-info/
+-rw-r--r--   0 mg         (501) wheel        (0)     4482 2023-05-14 12:34:06.000000 pypinyin-dict-0.6.0/src/pypinyin_dict.egg-info/PKG-INFO
+-rw-r--r--   0 mg         (501) wheel        (0)     2444 2023-05-14 12:34:06.000000 pypinyin-dict-0.6.0/src/pypinyin_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 mg         (501) wheel        (0)        1 2023-05-14 12:34:06.000000 pypinyin-dict-0.6.0/src/pypinyin_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 mg         (501) wheel        (0)        9 2023-05-14 12:34:06.000000 pypinyin-dict-0.6.0/src/pypinyin_dict.egg-info/requires.txt
+-rw-r--r--   0 mg         (501) wheel        (0)       14 2023-05-14 12:34:06.000000 pypinyin-dict-0.6.0/src/pypinyin_dict.egg-info/top_level.txt
```

### Comparing `pypinyin-dict-0.5.0/PKG-INFO` & `pypinyin-dict-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypinyin-dict
-Version: 0.5.0
+Version: 0.6.0
 Summary: 使用 pinyin-data 和 phrase-pinyin-data 中的拼音数据文件覆盖 pypinyin 中的自带拼音数据，实现只使用某个或某些拼音数据文件中的拼音数据的需求
 Home-page: https://github.com/mozillazg/pypinyin-dict
 Author: mozillazg
 Author-email: mozillazg101@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mozillazg/pypinyin-dict/issues
 Description: # pypinyin-dict
```

### Comparing `pypinyin-dict-0.5.0/README.md` & `pypinyin-dict-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/setup.py` & `pypinyin-dict-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="pypinyin-dict",
-    version="0.5.0",
+    version="0.6.0",
     author="mozillazg",
     author_email="mozillazg101@gmail.com",
     description="使用 pinyin-data 和 phrase-pinyin-data 中的拼音数据文件覆盖 pypinyin 中的自带拼音数据，实现只使用某个或某些拼音数据文件中的拼音数据的需求",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mozillazg/pypinyin-dict",
     project_urls={
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_0.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_0.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_1.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_1.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_2.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/cc_cedict_2.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/di.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/di.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_0.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1341,14 +1341,15 @@
     '一步八个谎': [['yī'], ['bù'], ['bā'], ['gè'], ['huǎng']],
     '一步到位': [['yī'], ['bù'], ['dào'], ['wèi']],
     '一步步': [['yí'], ['bù'], ['bù']],
     '一步步地': [['yí'], ['bù'], ['bù'], ['de']],
     '一步登天': [['yī'], ['bù'], ['dēng'], ['tiān']],
     '一步裙': [['yī'], ['bù'], ['qún']],
     '一死一生': [['yī'], ['sǐ'], ['yī'], ['shēng']],
+    '一死了之': [['yī'], ['sǐ'], ['liǎo'], ['zhī']],
     '一死儿': [['yī'], ['sǐ'], ['ér']],
     '一死生': [['yī'], ['sǐ'], ['shēng']],
     '一死的': [['yī'], ['sǐ'], ['de']],
     '一段': [['yī'], ['duàn']],
     '一殿': [['yī'], ['diàn']],
     '一毂辘': [['yī'], ['gū'], ['lù']],
     '一比': [['yī'], ['bǐ']],
@@ -41192,15 +41193,14 @@
     '克日': [['kè'], ['rì']],
     '克昌': [['kè'], ['chāng']],
     '克明': [['kè'], ['míng']],
     '克易': [['kè'], ['yì']],
     '克星': [['kè'], ['xīng']],
     '克暴': [['kè'], ['bào']],
     '克服': [['kè'], ['fú']],
-    '克朗': [['kè'], ['lǎng']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_1.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '克朗': [['kè'], ['lǎng']],
     '克朗代克': [['kè'], ['lǎng'], ['dài'], ['kè']],
     '克期': [['kè'], ['qī']],
     '克杀': [['kè'], ['shā']],
     '克构': [['kè'], ['gòu']],
     '克林姆': [['kè'], ['lín'], ['mǔ']],
     '克林姆酱': [['kè'], ['lín'], ['mǔ'], ['jiàng']],
     '克林德': [['kè'], ['lín'], ['dé']],
@@ -41192,15 +41193,14 @@
     '唯唯': [['wěi'], ['wěi']],
     '唯唯否否': [['wěi'], ['wěi'], ['fǒu'], ['fǒu']],
     '唯唯诺诺': [['wéi'], ['wéi'], ['nuò'], ['nuò']],
     '唯唯连声': [['wěi'], ['wěi'], ['lián'], ['shēng']],
     '唯喏': [['wéi'], ['nuò']],
     '唯复': [['wéi'], ['fù']],
     '唯妙唯肖': [['wéi'], ['miào'], ['wéi'], ['xiāo']],
-    '唯心': [['wéi'], ['xīn']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_2.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '唯心': [['wéi'], ['xīn']],
     '唯心主义': [['wéi'], ['xīn'], ['zhǔ'], ['yì']],
     '唯心史观': [['wéi'], ['xīn'], ['shǐ'], ['guān']],
     '唯心论': [['wéi'], ['xīn'], ['lùn']],
     '唯心辩证法': [['wéi'], ['xīn'], ['biàn'], ['zhèng'], ['fǎ']],
     '唯恐': [['wéi'], ['kǒng']],
     '唯恐天下不乱': [['wéi'], ['kǒng'], ['tiān'], ['xià'], ['bú'], ['luàn']],
     '唯意志论': [['wéi'], ['yì'], ['zhì'], ['lùn']],
@@ -15920,15 +15921,15 @@
     '太姒': [['tài'], ['sì']],
     '太婆': [['tài'], ['pó']],
     '太嫔': [['tài'], ['pín']],
     '太子': [['tài'], ['zǐ']],
     '太子丹': [['tài'], ['zǐ'], ['dān']],
     '太子党': [['tài'], ['zǐ'], ['dǎng']],
     '太子十三峰': [['tài'], ['zǐ'], ['shí'], ['sān'], ['fēng']],
-    '太子参': [['tài'], ['zi'], ['cān']],
+    '太子参': [['tài'], ['zi'], ['shēn']],
     '太子太保': [['tài'], ['zǐ'], ['tài'], ['bǎo']],
     '太子河区': [['tài'], ['zǐ'], ['hé'], ['qū']],
     '太子洗马': [['tài'], ['zǐ'], ['xǐ'], ['mǎ']],
     '太子港': [['tài'], ['zǐ'], ['gǎng']],
     '太孙': [['tài'], ['sūn']],
     '太学': [['tài'], ['xué']],
     '太学体': [['tài'], ['xué'], ['tǐ']],
@@ -41192,15 +41193,14 @@
     '巡警': [['xún'], ['jǐng']],
     '巡访': [['xún'], ['fǎng']],
     '巡诊': [['xún'], ['zhěn']],
     '巡边': [['xún'], ['biān']],
     '巡远': [['xún'], ['yuǎn']],
     '巡迣': [['xún'], ['zhì']],
     '巡迾': [['xún'], ['liè']],
-    '巡逴': [['xún'], ['chuò']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_3.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '巡逴': [['xún'], ['chuò']],
     '巡逻': [['xún'], ['luó']],
     '巡逻船': [['xún'], ['luó'], ['chuán']],
     '巡逻艇': [['xún'], ['luó'], ['tǐng']],
     '巡逻车': [['xún'], ['luó'], ['chē']],
     '巡逻队': [['xún'], ['luó'], ['duì']],
     '巡遁': [['xún'], ['dùn']],
     '巡道': [['xún'], ['dào']],
@@ -41192,15 +41193,14 @@
     '探讨': [['tàn'], ['tǎo']],
     '探讯': [['tàn'], ['xùn']],
     '探访': [['tàn'], ['fǎng']],
     '探询': [['tàn'], ['xún']],
     '探赏': [['tàn'], ['shǎng']],
     '探赜': [['tàn'], ['zé']],
     '探赜索隐': [['tàn'], ['zé'], ['suǒ'], ['yǐn']],
-    '探赜钩深': [['tàn'], ['zé'], ['gōu'], ['shēn']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_4.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '探赜钩深': [['tàn'], ['zé'], ['gōu'], ['shēn']],
     '探赤丸': [['tàn'], ['chì'], ['wán']],
     '探足': [['tàn'], ['zú']],
     '探路': [['tàn'], ['lù']],
     '探路者': [['tàn'], ['lù'], ['zhě']],
     '探身': [['tàn'], ['shēn']],
     '探身子': [['tàn'], ['shēn'], ['zi']],
     '探采': [['tàn'], ['cǎi']],
@@ -41192,15 +41193,14 @@
     '残疾儿童康复中心': [['cán'], ['jí'], ['ér'], ['tóng'], ['kāng'], ['fù'], ['zhōng'], ['xīn']],
     '残疾车': [['cán'], ['jí'], ['chē']],
     '残病': [['cán'], ['bìng']],
     '残破': [['cán'], ['pò']],
     '残碑': [['cán'], ['bēi']],
     '残碣': [['cán'], ['jié']],
     '残秋': [['cán'], ['qiū']],
-    '残租': [['cán'], ['zū']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_5.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '残租': [['cán'], ['zū']],
     '残秽': [['cán'], ['huì']],
     '残税': [['cán'], ['shuì']],
     '残稿': [['cán'], ['gǎo']],
     '残章断简': [['cán'], ['zhāng'], ['duàn'], ['jiǎn']],
     '残竹': [['cán'], ['zhú']],
     '残篇': [['cán'], ['piān']],
     '残篇断简': [['cán'], ['piān'], ['duàn'], ['jiǎn']],
@@ -41192,15 +41193,14 @@
     '画黛': [['huà'], ['dài']],
     '画黼': [['huà'], ['fǔ']],
     '画鼓': [['huà'], ['gǔ']],
     '画龙': [['huà'], ['lóng']],
     '画龙不成反为狗': [['huà'], ['lóng'], ['bù'], ['chéng'], ['fǎn'], ['wéi'], ['gǒu']],
     '画龙刻鹄': [['huà'], ['lóng'], ['kè'], ['hú']],
     '画龙点睛': [['huà'], ['lóng'], ['diǎn'], ['jīng']],
-    '画龙画虎难画骨': [['huà'], ['lóng'], ['huà'], ['hǔ'], ['nán'], ['huà'], ['gǔ']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_6.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_6.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '画龙画虎难画骨': [['huà'], ['lóng'], ['huà'], ['hǔ'], ['nán'], ['huà'], ['gǔ']],
     '甾酮': [['zāi'], ['tóng']],
     '甾醇': [['zāi'], ['chún']],
     '甿俗': [['méng'], ['sú']],
     '甿庶': [['méng'], ['shù']],
     '甿心': [['méng'], ['xīn']],
     '甿户': [['méng'], ['hù']],
     '甿歌': [['méng'], ['gē']],
@@ -41192,15 +41193,14 @@
     '罪恶深重': [['zuì'], ['è'], ['shēn'], ['zhòng']],
     '罪恶滔天': [['zuì'], ['è'], ['tāo'], ['tiān']],
     '罪恶的黑手': [['zuì'], ['è'], ['de'], ['hēi'], ['shǒu']],
     '罪恶贯盈': [['zuì'], ['è'], ['guàn'], ['yíng']],
     '罪恼': [['zuì'], ['nǎo']],
     '罪悔': [['zuì'], ['huǐ']],
     '罪情': [['zuì'], ['qíng']],
-    '罪愆': [['zuì'], ['qiān']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_7.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_7.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '罪愆': [['zuì'], ['qiān']],
     '罪慝': [['zuì'], ['tè']],
     '罪戮': [['zuì'], ['lù']],
     '罪戾': [['zuì'], ['lì']],
     '罪报': [['zuì'], ['bào']],
     '罪放': [['zuì'], ['fàng']],
     '罪文': [['zuì'], ['wén']],
     '罪有应得': [['zuì'], ['yǒu'], ['yīng'], ['dé']],
@@ -41192,15 +41193,14 @@
     '谭说': [['tán'], ['shuō']],
     '谭谭': [['tán'], ['tán']],
     '谭鑫培': [['tán'], ['xīn'], ['péi']],
     '谭震林': [['tán'], ['zhèn'], ['lín']],
     '谮下谩上': [['zèn'], ['xià'], ['mán'], ['shàng']],
     '谮人': [['zèn'], ['rén']],
     '谮妒': [['zèn'], ['dù']],
-    '谮害': [['zèn'], ['hài']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_8.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '谮害': [['zèn'], ['hài']],
     '谮恶': [['zèn'], ['è']],
     '谮愬': [['zèn'], ['shuò']],
     '谮慝': [['zèn'], ['tè']],
     '谮杀': [['zèn'], ['shā']],
     '谮构': [['zèn'], ['gòu']],
     '谮毁': [['zèn'], ['huǐ']],
     '谮润': [['zèn'], ['rùn']],
@@ -41192,15 +41193,14 @@
     '错文': [['cuò'], ['wén']],
     '错断': [['cuò'], ['duàn']],
     '错时': [['cuò'], ['shí']],
     '错明': [['cuò'], ['míng']],
     '错杂': [['cuò'], ['zá']],
     '错枉': [['cuò'], ['wǎng']],
     '错案': [['cuò'], ['àn']],
-    '错楚': [['cuò'], ['chǔ']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_9.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/large_pinyin_9.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 # Warning: Auto-generated file, don't edit.
 phrases_dict = {
+    '错楚': [['cuò'], ['chǔ']],
     '错比': [['cuò'], ['bǐ']],
     '错氛': [['cuò'], ['fēn']],
     '错法': [['cuò'], ['fǎ']],
     '错涂': [['cuò'], ['tú']],
     '错漏': [['cuò'], ['lòu']],
     '错漠': [['cuò'], ['mò']],
     '错然': [['cuò'], ['rán']],
@@ -41192,15 +41193,14 @@
     '龢鹊': [['hé'], ['què']],
     '龤声': [['xié'], ['shēng']],
     '𥆧息': [['shùn'], ['xī']],
     '𥻗子': [['chá'], ['zi']],
     '𥻗粥': [['chá'], ['zhōu']],
     '𩽾𩾌': [['ān'], ['kāng']],
     '𫚉鱼': [['hóng'], ['yú']],
-    '𫫇嗪': [['è'], ['qín']],
 }
 
 
 from pypinyin import load_phrases_dict
 
 
 def load():
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/pinyin.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/pinyin.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,14 +337,15 @@
     '一模二样': [['yī'], ['mó'], ['èr'], ['yàng']],
     '一次性': [['yí'], ['cì'], ['xìng']],
     '一步一个脚印': [['yī'], ['bù'], ['yī'], ['gè'], ['jiǎo'], ['yìn']],
     '一步一步': [['yí'], ['bù'], ['yí'], ['bù']],
     '一步一趋': [['yī'], ['bù'], ['yī'], ['qū']],
     '一步步': [['yí'], ['bù'], ['bù']],
     '一步步地': [['yí'], ['bù'], ['bù'], ['de']],
+    '一死了之': [['yī'], ['sǐ'], ['liǎo'], ['zhī']],
     '一毛不拔': [['yī'], ['máo'], ['bù'], ['bá']],
     '一毫不差': [['yī'], ['háo'], ['bù'], ['chā']],
     '一毫不染': [['yī'], ['háo'], ['bù'], ['rǎn']],
     '一毫不苟': [['yī'], ['háo'], ['bù'], ['gǒu']],
     '一民同俗': [['yī'], ['mín'], ['tóng'], ['sú']],
     '一气之下': [['yí'], ['qì'], ['zhī'], ['xià']],
     '一气呵成': [['yī'], ['qì'], ['hē'], ['chéng']],
@@ -5004,14 +5005,15 @@
     '佛爷': [['fó'], ['yé']],
     '佛牙': [['fó'], ['yá']],
     '佛珠': [['fó'], ['zhū']],
     '佛甲草': [['fó'], ['jiǎ'], ['cǎo']],
     '佛眼佛心': [['fó'], ['yǎn'], ['fó'], ['xīn']],
     '佛眼相看': [['fó'], ['yǎn'], ['xiāng'], ['kàn']],
     '佛祖': [['fó'], ['zǔ']],
+    '佛系': [['fó'], ['xì']],
     '佛经': [['fó'], ['jīng']],
     '佛罗伦萨': [['fó'], ['luó'], ['lún'], ['sà']],
     '佛门': [['fó'], ['mén']],
     '佛门弟子': [['fó'], ['mén'], ['dì'], ['zǐ']],
     '佛陀': [['fó'], ['tuó']],
     '佛龛': [['fó'], ['kān']],
     '作为': [['zuò'], ['wéi']],
@@ -14422,15 +14424,15 @@
     '太上皇': [['tài'], ['shàng'], ['huáng']],
     '太上老君': [['tài'], ['shàng'], ['lǎo'], ['jūn']],
     '太丘道广': [['tài'], ['qiū'], ['dào'], ['guǎng']],
     '太冲': [['tài'], ['chòng']],
     '太和': [['tài'], ['hé']],
     '太和殿': [['tài'], ['hé'], ['diàn']],
     '太夫人': [['tài'], ['fū'], ['rén']],
-    '太子参': [['tài'], ['zi'], ['cān']],
+    '太子参': [['tài'], ['zi'], ['shēn']],
     '太子港': [['tài'], ['zǐ'], ['gǎng']],
     '太尉': [['tài'], ['wèi']],
     '太山北斗': [['tài'], ['shān'], ['běi'], ['dòu']],
     '太岁头上动土': [['tài'], ['suì'], ['tóu'], ['shàng'], ['dòng'], ['tǔ']],
     '太师椅': [['tài'], ['shī'], ['yǐ']],
     '太平盛世': [['tài'], ['píng'], ['shèng'], ['shì']],
     '太平间': [['tài'], ['píng'], ['jiān']],
@@ -33238,14 +33240,15 @@
     '称心': [['chèn'], ['xīn']],
     '称心如意': [['chèn'], ['xīn'], ['rú'], ['yì']],
     '称心快意': [['chèn'], ['xīn'], ['kuài'], ['yì']],
     '称心满意': [['chèn'], ['xīn'], ['mǎn'], ['yì']],
     '称快': [['chēng'], ['kuài']],
     '称意': [['chēng'], ['yì']],
     '称愿': [['chèn'], ['yuàn']],
+    '称手': [['chèn'], ['shǒu']],
     '称扬': [['chēng'], ['yáng']],
     '称柴而爨': [['chēng'], ['chái'], ['ér'], ['cuàn']],
     '称王': [['chēng'], ['wáng']],
     '称王称霸': [['chēng'], ['wáng'], ['chēng'], ['bà']],
     '称病': [['chēng'], ['bìng']],
     '称绝': [['chēng'], ['jué']],
     '称羡': [['chēng'], ['xiàn']],
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_0.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_0.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_1.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_1.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_2.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_2.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_3.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_3.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_4.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_4.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_5.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_5.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_6.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_6.py`

 * *Files 0% similar despite different names*

```diff
@@ -31870,15 +31870,15 @@
     '进运': [['jìn'], ['yùn']],
     '进近': [['jìn'], ['jìn']],
     '进进': [['jìn'], ['jìn']],
     '进进出出': [['jìn'], ['jìn'], ['chū'], ['chū']],
     '进迫': [['jìn'], ['pò']],
     '进退': [['jìn'], ['tuì']],
     '进退两端': [['jìn'], ['tuì'], ['liǎng'], ['duān']],
-    '进退两难': [['jǐn'], ['tuì'], ['liǎng'], ['nán']],
+    '进退两难': [['jìn'], ['tuì'], ['liǎng'], ['nán']],
     '进退中度': [['jìn'], ['tuì'], ['zhòng'], ['dù']],
     '进退中绳': [['jìn'], ['tuì'], ['zhōng'], ['shéng']],
     '进退为难': [['jìn'], ['tuì'], ['wéi'], ['nán']],
     '进退亡据': [['jìn'], ['tuì'], ['wáng'], ['jù']],
     '进退出处': [['jìn'], ['tuì'], ['chū'], ['chǔ']],
     '进退双难': [['jìn'], ['tuì'], ['shuāng'], ['nán']],
     '进退可否': [['jìn'], ['tuì'], ['kě'], ['fǒu']],
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_7.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cibs_7.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_0.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_0.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_1.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_1.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_2.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/phrase_pinyin_data/zdic_cybs_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -6135,15 +6135,15 @@
     '进贤退奸': [['jìn'], ['xián'], ['tuì'], ['jiān']],
     '进贤退愚': [['jìn'], ['xián'], ['tuì'], ['yú']],
     '进贤黜佞': [['jìn'], ['xián'], ['chù'], ['nìng']],
     '进贤黜奸': [['jìn'], ['xián'], ['chù'], ['jiān']],
     '进贤黜恶': [['jìn'], ['xián'], ['chù'], ['è']],
     '进身之阶': [['jìn'], ['shēn'], ['zhī'], ['jiē']],
     '进退两端': [['jìn'], ['tuì'], ['liǎng'], ['duān']],
-    '进退两难': [['jǐn'], ['tuì'], ['liǎng'], ['nán']],
+    '进退两难': [['jìn'], ['tuì'], ['liǎng'], ['nán']],
     '进退中度': [['jìn'], ['tuì'], ['zhòng'], ['dù']],
     '进退中绳': [['jìn'], ['tuì'], ['zhōng'], ['shéng']],
     '进退为难': [['jìn'], ['tuì'], ['wéi'], ['nán']],
     '进退亡据': [['jìn'], ['tuì'], ['wáng'], ['jù']],
     '进退出处': [['jìn'], ['tuì'], ['chū'], ['chǔ']],
     '进退双难': [['jìn'], ['tuì'], ['shuāng'], ['nán']],
     '进退可否': [['jìn'], ['tuì'], ['kě'], ['fǒu']],
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/cc_cedict.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/cc_cedict.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/khanyupinlu.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/khanyupinlu.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/khanyupinyin.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/khanyupinyin.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/kmandarin_8105.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/kmandarin_8105.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/ktghz2013.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/ktghz2013.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/kxhc1983.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/kxhc1983.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/pinyin.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/pinyin.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict/pinyin_data/zdic.py` & `pypinyin-dict-0.6.0/src/pypinyin_dict/pinyin_data/zdic.py`

 * *Files identical despite different names*

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict.egg-info/PKG-INFO` & `pypinyin-dict-0.6.0/src/pypinyin_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypinyin-dict
-Version: 0.5.0
+Version: 0.6.0
 Summary: 使用 pinyin-data 和 phrase-pinyin-data 中的拼音数据文件覆盖 pypinyin 中的自带拼音数据，实现只使用某个或某些拼音数据文件中的拼音数据的需求
 Home-page: https://github.com/mozillazg/pypinyin-dict
 Author: mozillazg
 Author-email: mozillazg101@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mozillazg/pypinyin-dict/issues
 Description: # pypinyin-dict
```

### Comparing `pypinyin-dict-0.5.0/src/pypinyin_dict.egg-info/SOURCES.txt` & `pypinyin-dict-0.6.0/src/pypinyin_dict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

