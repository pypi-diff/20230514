# Comparing `tmp/xklb-1.26.30.tar.gz` & `tmp/xklb-1.26.31.tar.gz`

## Comparing `xklb-1.26.30.tar` & `xklb-1.26.31.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.30/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.30/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.30/Windows.md
--rw-r--r--   0        0        0   417004 2020-02-02 00:00:00.000000 xklb-1.26.30/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.30/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.30/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.30/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.30/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.26.30/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.26.30/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/books.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/consts.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/dl_config.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/lb.py
--rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/playback.py
--rw-r--r--   0        0        0    26800 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/praw_extract.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.30/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.30/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.30/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.30/LICENSE
--rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.26.30/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.30/pyproject.toml
--rw-r--r--   0        0        0    44036 2020-02-02 00:00:00.000000 xklb-1.26.30/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.31/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.31/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.31/Windows.md
+-rw-r--r--   0        0        0   417004 2020-02-02 00:00:00.000000 xklb-1.26.31/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.31/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.31/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.31/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.31/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.26.31/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.26.31/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/books.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/consts.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/dl_config.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/lb.py
+-rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/playback.py
+-rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21901 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.31/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.31/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.31/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.31/LICENSE
+-rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.26.31/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.31/pyproject.toml
+-rw-r--r--   0        0        0    44036 2020-02-02 00:00:00.000000 xklb-1.26.31/PKG-INFO
```

### Comparing `xklb-1.26.30/Windows.md` & `xklb-1.26.31/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/pdm.lock` & `xklb-1.26.31/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/readme.py` & `xklb-1.26.31/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.31/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.31/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/.github/workflows/push.yaml` & `xklb-1.26.31/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/sql/transfer.sql` & `xklb-1.26.31/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/av.py` & `xklb-1.26.31/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/books.py` & `xklb-1.26.31/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/consts.py` & `xklb-1.26.31/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/db.py` & `xklb-1.26.31/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/dl_config.py` & `xklb-1.26.31/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/dl_extract.py` & `xklb-1.26.31/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/fs_extract.py` & `xklb-1.26.31/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/gui.py` & `xklb-1.26.31/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/hn_extract.py` & `xklb-1.26.31/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/lb.py` & `xklb-1.26.31/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/play_actions.py` & `xklb-1.26.31/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/playback.py` & `xklb-1.26.31/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/player.py` & `xklb-1.26.31/xklb/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,28 +37,35 @@
 
 
 def calculate_duration(args, m) -> Tuple[int, int]:
     start = 0
     end = m.get("duration", 0)
     minimum_duration = 7 * 60
 
+    duration = m.get("duration", 20 * 60)
     if args.start:
         playhead = m.get("playhead")
 
         if args.start.isnumeric() and int(args.start) > 0:
             start = int(args.start)
+        elif args.start.endswith("%") and duration:
+            start_percent = int(args.start[:-1])
+            start = int(duration * start_percent / 100)
         elif playhead and any([end == 0, end > minimum_duration]):
             start = playhead
         elif args.start == "wadsworth":
-            start = m["duration"] * 0.3
+            start = duration * 0.3
         else:
             start = int(args.start)
     if args.end:
         if args.end == "dawsworth":
-            end = m["duration"] * 0.65
+            end = duration * 0.65
+        elif args.end.endswith("%") and duration:
+            end_percent = int(args.end[:-1])
+            end = int(duration * end_percent / 100)
         elif "+" in args.end:
             end = int(args.start) + int(args.end)
         else:
             end = int(args.end)
 
     return start, end
```

### Comparing `xklb-1.26.30/xklb/praw_extract.py` & `xklb-1.26.31/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/stats.py` & `xklb-1.26.31/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/subtitle.py` & `xklb-1.26.31/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/tabs_actions.py` & `xklb-1.26.31/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/tabs_extract.py` & `xklb-1.26.31/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/tube_backend.py` & `xklb-1.26.31/xklb/tube_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,15 +588,15 @@
     if match_filter_user_config is not None:
         match_filters.append(match_filter_user_config)
     ydl_opts["match_filter"] = yt_dlp.utils.match_filter_func(" & ".join(match_filters).split(" | "))
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         try:
             info = ydl.extract_info(m["path"], download=True)
-        except yt_dlp.DownloadError as e:
+        except (yt_dlp.DownloadError, ConnectionResetError) as e:
             error = consts.REGEX_ANSI_ESCAPE.sub("", str(e))
             ydl_log["error"].append(error)
             info = None
             log.debug("[%s]: yt-dlp %s", m["path"], error)
             # save_tube_entry(args, m, error=error)
             # return
```

### Comparing `xklb-1.26.30/xklb/tube_extract.py` & `xklb-1.26.31/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/utils.py` & `xklb-1.26.31/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/__init__.py` & `xklb-1.26.31/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/bigdirs.py` & `xklb-1.26.31/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/christen.py` & `xklb-1.26.31/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/copy_play_counts.py` & `xklb-1.26.31/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/dedupe.py` & `xklb-1.26.31/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/merge_dbs.py` & `xklb-1.26.31/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/merge_online_local.py` & `xklb-1.26.31/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/move_list.py` & `xklb-1.26.31/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/optimize_db.py` & `xklb-1.26.31/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/redownload.py` & `xklb-1.26.31/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/relmv.py` & `xklb-1.26.31/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/scatter.py` & `xklb-1.26.31/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.31/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/mining/data.py` & `xklb-1.26.31/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/mining/extract_links.py` & `xklb-1.26.31/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/mining/nouns.py` & `xklb-1.26.31/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/mining/pushshift.py` & `xklb-1.26.31/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.26.31/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/assets/kotobago.png` & `xklb-1.26.31/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/.gitignore` & `xklb-1.26.31/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/LICENSE` & `xklb-1.26.31/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/README.md` & `xklb-1.26.31/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.030)
+    xk media library subcommands (v1.26.031)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.26.30/pyproject.toml` & `xklb-1.26.31/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.30/PKG-INFO` & `xklb-1.26.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.30
+Version: 1.26.31
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
-    xk media library subcommands (v1.26.030)
+    xk media library subcommands (v1.26.031)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

