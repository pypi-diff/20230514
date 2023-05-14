# Comparing `tmp/xklb-1.27.2.tar.gz` & `tmp/xklb-1.27.3.tar.gz`

## Comparing `xklb-1.27.2.tar` & `xklb-1.27.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.2/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.2/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.2/Windows.md
--rw-r--r--   0        0        0   416092 2020-02-02 00:00:00.000000 xklb-1.27.2/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.2/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.2/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.2/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/books.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/consts.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/dl_config.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/lb.py
--rw-r--r--   0        0        0    35715 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/playback.py
--rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/praw_extract.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.2/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.2/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.2/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.2/LICENSE
--rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.2/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.2/pyproject.toml
--rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.3/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.3/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.3/Windows.md
+-rw-r--r--   0        0        0   416092 2020-02-02 00:00:00.000000 xklb-1.27.3/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.3/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.3/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.3/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/books.py
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/consts.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/dl_config.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/lb.py
+-rw-r--r--   0        0        0    35715 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/playback.py
+-rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.3/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.3/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.3/LICENSE
+-rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.3/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.3/pyproject.toml
+-rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.3/PKG-INFO
```

### Comparing `xklb-1.27.2/Windows.md` & `xklb-1.27.3/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/pdm.lock` & `xklb-1.27.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/readme.py` & `xklb-1.27.3/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.27.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.27.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/.github/workflows/push.yaml` & `xklb-1.27.3/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/sql/transfer.sql` & `xklb-1.27.3/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/av.py` & `xklb-1.27.3/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/books.py` & `xklb-1.27.3/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/consts.py` & `xklb-1.27.3/xklb/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-import enum, os, re, sys
+import enum, os, re, secrets, string, sys
 from datetime import datetime, timezone
 from pathlib import Path
 from tempfile import gettempdir
 from types import SimpleNamespace
 from typing import List
 
 
 def now():
     return int(datetime.now(tz=timezone.utc).timestamp())
 
 
+def random_string(length=5):
+    return "".join(secrets.choice(string.ascii_letters + string.digits) for _ in range(length))
+
+
 TEMP_DIR = gettempdir()
 FAKE_SUBTITLE = str(Path(TEMP_DIR) / "sub.srt")  # https://github.com/skorokithakis/catt/issues/393
 CAST_NOW_PLAYING = str(Path(TEMP_DIR) / "catt_playing")
 DEFAULT_MPV_SOCKET = str(Path(TEMP_DIR) / "mpv_socket")
 DEFAULT_MPV_WATCH_LATER = str(Path("~/.config/mpv/watch_later/").expanduser().resolve())
-SUB_TEMP_DIR = str(Path(TEMP_DIR) / "library_temp_subtitles")
+SUB_TEMP_DIR = str(Path(TEMP_DIR) / "library_temp_subtitles" / random_string())
 BLOCK_THE_CHANNEL = "__BLOCKLIST_ENTRY_"
 
 LOG_INFO = 1
 LOG_DEBUG = 2
 SIMILAR = 1
 SIMILAR_NO_FILTER = 2
 SIMILAR_NO_FILTER_NO_FTS = 2
```

### Comparing `xklb-1.27.2/xklb/db.py` & `xklb-1.27.3/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/dl_config.py` & `xklb-1.27.3/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/dl_extract.py` & `xklb-1.27.3/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/fs_extract.py` & `xklb-1.27.3/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/gui.py` & `xklb-1.27.3/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/hn_extract.py` & `xklb-1.27.3/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/lb.py` & `xklb-1.27.3/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/play_actions.py` & `xklb-1.27.3/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/playback.py` & `xklb-1.27.3/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/player.py` & `xklb-1.27.3/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/praw_extract.py` & `xklb-1.27.3/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/stats.py` & `xklb-1.27.3/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/subtitle.py` & `xklb-1.27.3/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/tabs_actions.py` & `xklb-1.27.3/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/tabs_extract.py` & `xklb-1.27.3/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/tube_backend.py` & `xklb-1.27.3/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/tube_extract.py` & `xklb-1.27.3/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/utils.py` & `xklb-1.27.3/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/__init__.py` & `xklb-1.27.3/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/bigdirs.py` & `xklb-1.27.3/xklb/scripts/bigdirs.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,22 +51,22 @@
         while len(p) >= 2:
             p.pop()
             parent = "/".join(p) + "/"
 
             file_deleted = bool(m.get("time_deleted", 0))
             file_played = bool(m.get("time_played", 0))
             if parent not in d:
-                d[parent] = {"size": 0, "count": 0, "count_deleted": 0, "count_played": 0}
+                d[parent] = {"size": 0, "count": 0, "deleted": 0, "played": 0}
             if not file_deleted:
                 d[parent]["size"] += m.get("size", 0)
                 d[parent]["count"] += 1
             else:
-                d[parent]["count_deleted"] += 1
+                d[parent]["deleted"] += 1
             if file_played:
-                d[parent]["count_played"] += 1
+                d[parent]["played"] += 1
 
     for path, pdict in list(d.items()):
         if pdict["count"] == 0:
             d.pop(path)
         elif not args.depth:
             if pdict["count"] < (args.lower or 4):
                 d.pop(path)
@@ -86,16 +86,16 @@
         parent = "/".join(p[:depth]) + "/"
         if len(p) < depth:
             continue
 
         if d.get(parent):
             d[parent]["size"] += f["size"]
             d[parent]["count"] += f["count"]
-            d[parent]["count_deleted"] += f["count_deleted"]
-            d[parent]["count_played"] += f["count_played"]
+            d[parent]["deleted"] += f["deleted"]
+            d[parent]["played"] += f["played"]
         else:
             d[parent] = f
 
     for path, pdict in list(d.items()):
         if args.lower is not None and pdict["count"] < args.lower:
             d.pop(path)
         elif args.upper is not None and pdict["count"] > args.upper:
@@ -125,19 +125,20 @@
     )
     return media
 
 
 def sort_by(args):
     if args.sort_by:
         if args.sort_by == "played_ratio":
-            return lambda x: x["count_played"] / x["count_deleted"] if x["count_deleted"] else 0
+            return lambda x: x["played"] / x["deleted"] if x["deleted"] else 0
         elif args.sort_by == "deleted_ratio":
-            return lambda x: x["count_deleted"] / x["count_played"] if x["count_played"] else 0
+            return lambda x: x["deleted"] / x["played"] if x["played"] else 0
         else:
-            return lambda x: x[f"count_{args.sort_by}"]
+            return lambda x: x[args.sort_by]
+
     return lambda x: x["size"] / x["count"]
 
 
 def process_bigdirs(args, media) -> List[Dict]:
     folders = group_files_by_folder(args, media)
     if args.depth:
         folders = group_folders(args, folders)
```

### Comparing `xklb-1.27.2/xklb/scripts/christen.py` & `xklb-1.27.3/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/copy_play_counts.py` & `xklb-1.27.3/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/dedupe.py` & `xklb-1.27.3/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/merge_dbs.py` & `xklb-1.27.3/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/merge_online_local.py` & `xklb-1.27.3/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/move_list.py` & `xklb-1.27.3/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/optimize_db.py` & `xklb-1.27.3/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/redownload.py` & `xklb-1.27.3/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/relmv.py` & `xklb-1.27.3/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/scatter.py` & `xklb-1.27.3/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/streaming_tab_loader.py` & `xklb-1.27.3/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/mining/data.py` & `xklb-1.27.3/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/mining/extract_links.py` & `xklb-1.27.3/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/mining/nouns.py` & `xklb-1.27.3/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/mining/pushshift.py` & `xklb-1.27.3/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.27.3/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/assets/kotobago.png` & `xklb-1.27.3/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/.gitignore` & `xklb-1.27.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/LICENSE` & `xklb-1.27.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/README.md` & `xklb-1.27.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.27.002)
+    xk media library subcommands (v1.27.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.27.2/pyproject.toml` & `xklb-1.27.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.27.2/PKG-INFO` & `xklb-1.27.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.27.2
+Version: 1.27.3
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
-    xk media library subcommands (v1.27.002)
+    xk media library subcommands (v1.27.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

