# Comparing `tmp/xklb-1.26.31.tar.gz` & `tmp/xklb-1.27.2.tar.gz`

## Comparing `xklb-1.26.31.tar` & `xklb-1.27.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.31/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.31/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.31/Windows.md
--rw-r--r--   0        0        0   417004 2020-02-02 00:00:00.000000 xklb-1.26.31/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.31/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.31/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.31/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.31/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.26.31/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.26.31/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/books.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/consts.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/dl_config.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/lb.py
--rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/playback.py
--rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/praw_extract.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21901 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.31/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.31/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.31/LICENSE
--rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.26.31/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.31/pyproject.toml
--rw-r--r--   0        0        0    44036 2020-02-02 00:00:00.000000 xklb-1.26.31/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.2/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.2/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.2/Windows.md
+-rw-r--r--   0        0        0   416092 2020-02-02 00:00:00.000000 xklb-1.27.2/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.2/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.2/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.2/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/books.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/consts.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/dl_config.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/lb.py
+-rw-r--r--   0        0        0    35715 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/playback.py
+-rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.2/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.2/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.2/LICENSE
+-rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.2/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.2/pyproject.toml
+-rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.2/PKG-INFO
```

### Comparing `xklb-1.26.31/Windows.md` & `xklb-1.27.2/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/pdm.lock` & `xklb-1.27.2/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -771,24 +771,14 @@
 
 [[package]]
 name = "pytz"
 version = "2023.3"
 summary = "World timezone definitions, modern and historical"
 
 [[package]]
-name = "pytz-deprecation-shim"
-version = "0.1.0.post0"
-requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7"
-summary = "Shims to make deprecation of pytz easier"
-dependencies = [
-    "backports-zoneinfo; python_version >= \"3.6\" and python_version < \"3.9\"",
-    "tzdata; python_version >= \"3.6\"",
-]
-
-[[package]]
 name = "rarfile"
 version = "4.0"
 summary = "RAR archive reader for Python"
 
 [[package]]
 name = "rebulk"
 version = "3.2.0"
@@ -992,20 +982,19 @@
 name = "tzdata"
 version = "2023.3"
 requires_python = ">=2"
 summary = "Provider of IANA time zone data"
 
 [[package]]
 name = "tzlocal"
-version = "4.3"
+version = "5.0"
 requires_python = ">=3.7"
 summary = "tzinfo object for the local timezone"
 dependencies = [
     "backports-zoneinfo; python_version < \"3.9\"",
-    "pytz-deprecation-shim",
     "tzdata; platform_system == \"Windows\"",
 ]
 
 [[package]]
 name = "update-checker"
 version = "0.18.0"
 summary = "A python module that will check for package updates."
@@ -2446,18 +2435,14 @@
 "python-pptx 0.6.21" = [
     {url = "https://files.pythonhosted.org/packages/eb/c3/bd8f2316a790291ef5aa5225c740fa60e2cf754376e90cb1a44fde056830/python-pptx-0.6.21.tar.gz", hash = "sha256:7798a2aaf89563565b3c7120c0acfe9aff775db0db3580544e3bf4840c2e378f"},
 ]
 "pytz 2023.3" = [
     {url = "https://files.pythonhosted.org/packages/5e/32/12032aa8c673ee16707a9b6cdda2b09c0089131f35af55d443b6a9c69c1d/pytz-2023.3.tar.gz", hash = "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588"},
     {url = "https://files.pythonhosted.org/packages/7f/99/ad6bd37e748257dd70d6f85d916cafe79c0b0f5e2e95b11f7fbc82bf3110/pytz-2023.3-py2.py3-none-any.whl", hash = "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"},
 ]
-"pytz-deprecation-shim 0.1.0.post0" = [
-    {url = "https://files.pythonhosted.org/packages/94/f0/909f94fea74759654390a3e1a9e4e185b6cd9aa810e533e3586f39da3097/pytz_deprecation_shim-0.1.0.post0.tar.gz", hash = "sha256:af097bae1b616dde5c5744441e2ddc69e74dfdcb0c263129610d85b87445a59d"},
-    {url = "https://files.pythonhosted.org/packages/eb/73/3eaab547ca809754e67e06871cff0fc962bafd4b604e15f31896a0f94431/pytz_deprecation_shim-0.1.0.post0-py2.py3-none-any.whl", hash = "sha256:8314c9692a636c8eb3bda879b9f119e350e93223ae83e70e80c31675a0fdc1a6"},
-]
 "rarfile 4.0" = [
     {url = "https://files.pythonhosted.org/packages/0c/2f/894bc187ce40367f2e878ced196e1b5a9bc66cb553a062ed955d4f7dcbab/rarfile-4.0.tar.gz", hash = "sha256:67548769229c5bda0827c1663dce3f54644f9dbfba4ae86d4da2b2afd3e602a1"},
     {url = "https://files.pythonhosted.org/packages/95/f4/c92fab227c7457e3b76a4096ccb655ded9deac869849cb03afbe55dfdc1e/rarfile-4.0-py3-none-any.whl", hash = "sha256:1094869119012f95c31a6f22cc3a9edbdca61861b805241116adbe2d737b68f8"},
 ]
 "rebulk 3.2.0" = [
     {url = "https://files.pythonhosted.org/packages/84/4d/df073d593f7e7e4a5a7e19148b2e9b4ae63b4ddcbb863f1e7bb2b6f19c62/rebulk-3.2.0-py3-none-any.whl", hash = "sha256:6bc31ae4b37200623c5827d2f539f9ec3e52b50431322dad8154642a39b0a53e"},
     {url = "https://files.pythonhosted.org/packages/f2/06/24c69f8d707c9eefc1108a64e079da56b5f351e3f59ed76e8f04b9f3e296/rebulk-3.2.0.tar.gz", hash = "sha256:0d30bf80fca00fa9c697185ac475daac9bde5f646ce3338c9ff5d5dc1ebdfebc"},
@@ -2662,17 +2647,17 @@
     {url = "https://files.pythonhosted.org/packages/31/25/5abcd82372d3d4a3932e1fa8c3dbf9efac10cc7c0d16e78467460571b404/typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
     {url = "https://files.pythonhosted.org/packages/d3/20/06270dac7316220643c32ae61694e451c98f8caf4c8eab3aa80a2bedf0df/typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
 ]
 "tzdata 2023.3" = [
     {url = "https://files.pythonhosted.org/packages/70/e5/81f99b9fced59624562ab62a33df639a11b26c582be78864b339dafa420d/tzdata-2023.3.tar.gz", hash = "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a"},
     {url = "https://files.pythonhosted.org/packages/d5/fb/a79efcab32b8a1f1ddca7f35109a50e4a80d42ac1c9187ab46522b2407d7/tzdata-2023.3-py2.py3-none-any.whl", hash = "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"},
 ]
-"tzlocal 4.3" = [
-    {url = "https://files.pythonhosted.org/packages/39/97/b15b711a10d0774390404bec9712b2647b0b53a4da50a08acf7d7e51e284/tzlocal-4.3.tar.gz", hash = "sha256:3f21d09e1b2aa9f2dacca12da240ca37de3ba5237a93addfd6d593afe9073355"},
-    {url = "https://files.pythonhosted.org/packages/d4/46/e8002faae3d1df7d7a0a3aa0cb4b2ccd805c3a71fb507b06446012b28790/tzlocal-4.3-py3-none-any.whl", hash = "sha256:b44c4388f3d34f25862cfbb387578a4d70fec417649da694a132f628a23367e2"},
+"tzlocal 5.0" = [
+    {url = "https://files.pythonhosted.org/packages/0a/93/55e34fba4b61fd4ba30e9341edb313f474d0e18006e8400b05e36b71a7bd/tzlocal-5.0-py3-none-any.whl", hash = "sha256:c640e3fdccbb6fee1172ce211cefd3c3c04eaf2b0fbf676f0ac7958c41f373e4"},
+    {url = "https://files.pythonhosted.org/packages/23/0a/b3d3e8a9dd99e4a7789309de8ed12a625ed80efbe4f1cd4282efda88734e/tzlocal-5.0.tar.gz", hash = "sha256:f96e29a599ef562233cec21ef0d6f7065c3050d0221293e839d1ede093ab1755"},
 ]
 "update-checker 0.18.0" = [
     {url = "https://files.pythonhosted.org/packages/0c/ba/8dd7fa5f0b1c6a8ac62f8f57f7e794160c1f86f31c6d0fb00f582372a3e4/update_checker-0.18.0-py3-none-any.whl", hash = "sha256:cbba64760a36fe2640d80d85306e8fe82b6816659190993b7bdabadee4d4bbfd"},
     {url = "https://files.pythonhosted.org/packages/5c/0b/1bec4a6cc60d33ce93d11a7bcf1aeffc7ad0aa114986073411be31395c6f/update_checker-0.18.0.tar.gz", hash = "sha256:6a2d45bb4ac585884a6b03f9eade9161cedd9e8111545141e9aa9058932acb13"},
 ]
 "urllib3 1.25.11" = [
     {url = "https://files.pythonhosted.org/packages/56/aa/4ef5aa67a9a62505db124a5cb5262332d1d4153462eb8fd89c9fa41e5d92/urllib3-1.25.11-py2.py3-none-any.whl", hash = "sha256:f5321fbe4bf3fefa0efd0bfe7fb14e90909eb62a48ccda331726b4319897dd5e"},
```

### Comparing `xklb-1.26.31/readme.py` & `xklb-1.27.2/readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
 You may filter by folder depth (similar to QDirStat or WizTree)
 
     $ lb bigdirs --depth=3 audio.db
 
 There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
 
-    $ lb bigdirs --sort-by-deleted audio.db
+    $ lb bigdirs --sort-by deleted audio.db
 
 </details>
 
 
 ### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
 
 <details><summary>If you use mergerfs, you'll likely be interested in this</summary>
```

### Comparing `xklb-1.26.31/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.27.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.27.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/.github/workflows/push.yaml` & `xklb-1.27.2/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/sql/transfer.sql` & `xklb-1.27.2/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/av.py` & `xklb-1.27.2/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/books.py` & `xklb-1.27.2/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/consts.py` & `xklb-1.27.2/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/db.py` & `xklb-1.27.2/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/dl_config.py` & `xklb-1.27.2/xklb/dl_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 .*restricted
 .*Internal Server Error
 .*Internal error encountered
 .*not currently available
 .*currently unavailable
 .*selectionunavailable
 .*Downloaded .* bytes, expected .* bytes
+.*FileNotFoundError
 .*Playlists that require authentication may not extract correctly without a successful webpage download
 .*Main webpage is locked behind the login page
 .*You need to log in to access this content
 .*This video is only available for registered users
 .*members-only content
 .*not available in your location
 .*linked to an account
```

### Comparing `xklb-1.26.31/xklb/dl_extract.py` & `xklb-1.27.2/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/fs_extract.py` & `xklb-1.27.2/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/gui.py` & `xklb-1.27.2/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/hn_extract.py` & `xklb-1.27.2/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/lb.py` & `xklb-1.27.2/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/play_actions.py` & `xklb-1.27.2/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,15 @@
     parser.add_argument("--online-media-only", "--online-only", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--local-media-only", "--local-only", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
 
     parser.add_argument("--sibling", "--episode", action="store_true")
     parser.add_argument("--solo", action="store_true")
 
-    parser.add_argument("--sort-by-deleted", action="store_true")
+    parser.add_argument("--sort-by", action="store_true")
     parser.add_argument("--depth", "-D", default=0, type=int, help="Depth of folders")
     parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
 
     parser.add_argument("--timeout", "-T", help=argparse.SUPPRESS)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true")
```

### Comparing `xklb-1.26.31/xklb/playback.py` & `xklb-1.27.2/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/player.py` & `xklb-1.27.2/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/praw_extract.py` & `xklb-1.27.2/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/stats.py` & `xklb-1.27.2/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/subtitle.py` & `xklb-1.27.2/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/tabs_actions.py` & `xklb-1.27.2/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/tabs_extract.py` & `xklb-1.27.2/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/tube_backend.py` & `xklb-1.27.2/xklb/tube_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,15 +588,15 @@
     if match_filter_user_config is not None:
         match_filters.append(match_filter_user_config)
     ydl_opts["match_filter"] = yt_dlp.utils.match_filter_func(" & ".join(match_filters).split(" | "))
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         try:
             info = ydl.extract_info(m["path"], download=True)
-        except (yt_dlp.DownloadError, ConnectionResetError) as e:
+        except (yt_dlp.DownloadError, ConnectionResetError, FileNotFoundError) as e:
             error = consts.REGEX_ANSI_ESCAPE.sub("", str(e))
             ydl_log["error"].append(error)
             info = None
             log.debug("[%s]: yt-dlp %s", m["path"], error)
             # save_tube_entry(args, m, error=error)
             # return
```

### Comparing `xklb-1.26.31/xklb/tube_extract.py` & `xklb-1.27.2/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/utils.py` & `xklb-1.27.2/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/__init__.py` & `xklb-1.27.2/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/bigdirs.py` & `xklb-1.27.2/xklb/scripts/bigdirs.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from xklb import db, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library bigdirs",
-        usage="""library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by-deleted] [--size=+5MB]
+        usage="""library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by "deleted" | "played"] [--size=+5MB]
 
     See what folders take up space
 
         lb bigdirs video.db
         lb bigdirs audio.db
         lb bigdirs fs.db
 """,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--sort-by-deleted", action="store_true")
+    parser.add_argument("--sort-by")
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="4000")
     parser.add_argument("--depth", "-d", default=0, type=int, help="Depth of folders")
     parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
     parser.add_argument(
         "--size",
         "-S",
@@ -48,26 +48,25 @@
     d = {}
     for m in media:
         p = m["path"].split("/")
         while len(p) >= 2:
             p.pop()
             parent = "/".join(p) + "/"
 
-            file_exists = (m.get("time_deleted") or 0) == 0
-
-            if d.get(parent):
-                d[parent]["size"] += (m["size"] or 0) if file_exists else 0
-                d[parent]["count"] += 1 if file_exists else 0
-                d[parent]["count_deleted"] += 0 if file_exists else 1
+            file_deleted = bool(m.get("time_deleted", 0))
+            file_played = bool(m.get("time_played", 0))
+            if parent not in d:
+                d[parent] = {"size": 0, "count": 0, "count_deleted": 0, "count_played": 0}
+            if not file_deleted:
+                d[parent]["size"] += m.get("size", 0)
+                d[parent]["count"] += 1
             else:
-                d[parent] = {
-                    "size": (m["size"] or 0) if file_exists else 0,
-                    "count": 1 if file_exists else 0,
-                    "count_deleted": 0 if file_exists else 1,
-                }
+                d[parent]["count_deleted"] += 1
+            if file_played:
+                d[parent]["count_played"] += 1
 
     for path, pdict in list(d.items()):
         if pdict["count"] == 0:
             d.pop(path)
         elif not args.depth:
             if pdict["count"] < (args.lower or 4):
                 d.pop(path)
@@ -88,14 +87,15 @@
         if len(p) < depth:
             continue
 
         if d.get(parent):
             d[parent]["size"] += f["size"]
             d[parent]["count"] += f["count"]
             d[parent]["count_deleted"] += f["count_deleted"]
+            d[parent]["count_played"] += f["count_played"]
         else:
             d[parent] = f
 
     for path, pdict in list(d.items()):
         if args.lower is not None and pdict["count"] < args.lower:
             d.pop(path)
         elif args.upper is not None and pdict["count"] > args.upper:
@@ -110,42 +110,54 @@
     media = list(
         args.db.query(
             f"""
         select
             path
             , size
             {', time_deleted' if 'time_deleted' in columns else ''}
+            {', time_played' if 'time_played' in columns else ''}
         from media
         where 1=1
             {'and time_downloaded > 0' if 'time_downloaded' in columns else ''}
             {args.size if args.size else ''}
         order by path
         """,
         ),
     )
     return media
 
 
+def sort_by(args):
+    if args.sort_by:
+        if args.sort_by == "played_ratio":
+            return lambda x: x["count_played"] / x["count_deleted"] if x["count_deleted"] else 0
+        elif args.sort_by == "deleted_ratio":
+            return lambda x: x["count_deleted"] / x["count_played"] if x["count_played"] else 0
+        else:
+            return lambda x: x[f"count_{args.sort_by}"]
+    return lambda x: x["size"] / x["count"]
+
+
 def process_bigdirs(args, media) -> List[Dict]:
     folders = group_files_by_folder(args, media)
     if args.depth:
         folders = group_folders(args, folders)
-    return sorted(folders, key=lambda x: x["count_deleted"] if args.sort_by_deleted else x["size"] / x["count"])
+    return sorted(folders, key=sort_by(args))
 
 
 def bigdirs() -> None:
     args = parse_args()
     tbl = get_table(args)
     tbl = process_bigdirs(args, tbl)
 
     if args.limit:
         tbl = tbl[-int(args.limit) :]
 
     tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
-    tbl = utils.col_resize(tbl, "path", 60)
+    tbl = utils.col_resize(tbl, "path", 50)
     tbl = utils.col_naturalsize(tbl, "size")
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
     if not args.limit:
         print(f"{len(tbl)} folders found")
 
 
 if __name__ == "__main__":
```

### Comparing `xklb-1.26.31/xklb/scripts/christen.py` & `xklb-1.27.2/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/copy_play_counts.py` & `xklb-1.27.2/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/dedupe.py` & `xklb-1.27.2/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/merge_dbs.py` & `xklb-1.27.2/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/merge_online_local.py` & `xklb-1.27.2/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/move_list.py` & `xklb-1.27.2/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/optimize_db.py` & `xklb-1.27.2/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/redownload.py` & `xklb-1.27.2/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/relmv.py` & `xklb-1.27.2/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/scatter.py` & `xklb-1.27.2/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/streaming_tab_loader.py` & `xklb-1.27.2/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/mining/data.py` & `xklb-1.27.2/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/mining/extract_links.py` & `xklb-1.27.2/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/mining/nouns.py` & `xklb-1.27.2/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/mining/pushshift.py` & `xklb-1.27.2/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.27.2/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/assets/kotobago.png` & `xklb-1.27.2/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/.gitignore` & `xklb-1.27.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/LICENSE` & `xklb-1.27.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/README.md` & `xklb-1.27.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.031)
+    xk media library subcommands (v1.27.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -531,15 +531,15 @@
 
 You may filter by folder depth (similar to QDirStat or WizTree)
 
     $ lb bigdirs --depth=3 audio.db
 
 There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
 
-    $ lb bigdirs --sort-by-deleted audio.db
+    $ lb bigdirs --sort-by deleted audio.db
 
 </details>
 
 
 ### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
 
 <details><summary>If you use mergerfs, you'll likely be interested in this</summary>
```

### Comparing `xklb-1.26.31/pyproject.toml` & `xklb-1.27.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.31/PKG-INFO` & `xklb-1.27.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.31
+Version: 1.27.2
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.031)
+    xk media library subcommands (v1.27.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -613,15 +613,15 @@
 
 You may filter by folder depth (similar to QDirStat or WizTree)
 
     $ lb bigdirs --depth=3 audio.db
 
 There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
 
-    $ lb bigdirs --sort-by-deleted audio.db
+    $ lb bigdirs --sort-by deleted audio.db
 
 </details>
 
 
 ### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
 
 <details><summary>If you use mergerfs, you'll likely be interested in this</summary>
```

