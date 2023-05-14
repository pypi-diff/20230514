# Comparing `tmp/xklb-1.27.3.tar.gz` & `tmp/xklb-1.27.4.tar.gz`

## Comparing `xklb-1.27.3.tar` & `xklb-1.27.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.3/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.3/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.3/Windows.md
--rw-r--r--   0        0        0   416092 2020-02-02 00:00:00.000000 xklb-1.27.3/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.3/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.3/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.3/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/books.py
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/consts.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/dl_config.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/lb.py
--rw-r--r--   0        0        0    35715 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/playback.py
--rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/praw_extract.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.3/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.3/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.3/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.3/LICENSE
--rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.3/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.3/pyproject.toml
--rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.3/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.4/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.4/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.4/Windows.md
+-rw-r--r--   0        0        0   416092 2020-02-02 00:00:00.000000 xklb-1.27.4/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.4/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.4/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.4/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/books.py
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/consts.py
+-rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/lb.py
+-rw-r--r--   0        0        0    35208 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/playback.py
+-rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.4/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.4/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.4/LICENSE
+-rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.4/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.4/pyproject.toml
+-rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.4/PKG-INFO
```

### Comparing `xklb-1.27.3/Windows.md` & `xklb-1.27.4/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/pdm.lock` & `xklb-1.27.4/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/readme.py` & `xklb-1.27.4/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.27.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.27.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/.github/workflows/push.yaml` & `xklb-1.27.4/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/sql/transfer.sql` & `xklb-1.27.4/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/av.py` & `xklb-1.27.4/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/books.py` & `xklb-1.27.4/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/consts.py` & `xklb-1.27.4/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/db.py` & `xklb-1.27.4/xklb/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -209,14 +209,25 @@
     excl = ":exclude{0}"
     include_string = "AND (" + " OR ".join([f"{col} LIKE {incl}" for col in valid_cols]) + ")"
     exclude_string = "AND (" + " AND ".join([f"COALESCE({col},'') NOT LIKE {excl}" for col in valid_cols]) + ")"
 
     return include_string, exclude_string
 
 
+def construct_search_bindings(args, columns) -> None:
+    includes, excludes = gen_include_excludes(columns)
+
+    for idx, inc in enumerate(args.include):
+        args.filter_sql.append(includes.format(idx))
+        args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
+    for idx, exc in enumerate(args.exclude):
+        args.filter_sql.append(excludes.format(idx))
+        args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
+
+
 def get_playlists(args, cols="path, dl_config", constrain=False, sql_filters=None) -> List[dict]:
     columns = args.db["playlists"].columns_dict
     if sql_filters is None:
         sql_filters = []
     if "time_deleted" in columns:
         sql_filters.append("AND COALESCE(time_deleted,0) = 0")
     if constrain and args.category:
```

### Comparing `xklb-1.27.3/xklb/dl_config.py` & `xklb-1.27.4/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/dl_extract.py` & `xklb-1.27.4/xklb/dl_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     args.filter_bindings = {}
 
     if args.duration:
         args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
-    play_actions.construct_search_bindings(args, m_columns)
+    db.construct_search_bindings(args, m_columns)
 
     args.filter_sql.append(
         f"""and cast(STRFTIME('%s',
           datetime( COALESCE(time_modified,0), 'unixepoch', '+{args.retry_delay}')
         ) as int) < STRFTIME('%s', datetime()) """,
     )
```

### Comparing `xklb-1.27.3/xklb/fs_extract.py` & `xklb-1.27.4/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/gui.py` & `xklb-1.27.4/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/hn_extract.py` & `xklb-1.27.4/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/lb.py` & `xklb-1.27.4/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/play_actions.py` & `xklb-1.27.4/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,25 +495,14 @@
 
     utils.timeout(args.timeout)
 
     args.sock = None
     return args
 
 
-def construct_search_bindings(args, columns) -> None:
-    includes, excludes = db.gen_include_excludes(columns)
-
-    for idx, inc in enumerate(args.include):
-        args.filter_sql.append(includes.format(idx))
-        args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
-    for idx, exc in enumerate(args.exclude):
-        args.filter_sql.append(excludes.format(idx))
-        args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
-
-
 def construct_query(args) -> Tuple[str, dict]:
     m_columns = args.db["media"].columns_dict
     args.filter_sql = []
     args.filter_bindings = {}
 
     if args.duration:
         args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
@@ -568,17 +557,17 @@
 
     args.table = "media"
     if args.db["media"].detect_fts() and not args.no_fts:
         if args.include:
             args.table = db.fts_search(args)
             m_columns = {**m_columns, "rank": int}
         elif args.exclude:
-            construct_search_bindings(args, m_columns)
+            db.construct_search_bindings(args, m_columns)
     else:
-        construct_search_bindings(args, m_columns)
+        db.construct_search_bindings(args, m_columns)
 
     if args.table == "media" and not any(
         [
             args.filter_sql,
             args.where,
             args.print,
             args.partial,
```

### Comparing `xklb-1.27.3/xklb/playback.py` & `xklb-1.27.4/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/player.py` & `xklb-1.27.4/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/praw_extract.py` & `xklb-1.27.4/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/stats.py` & `xklb-1.27.4/xklb/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     args.filter_sql.extend([" and " + w for w in args.where])
 
     args.table = "playlists"
     if args.db["playlists"].detect_fts():
         if args.include:
             args.table = db.fts_search(args)
         elif args.exclude:
-            play_actions.construct_search_bindings(args, pl_columns)
+            db.construct_search_bindings(args, pl_columns)
     else:
-        play_actions.construct_search_bindings(args, pl_columns)
+        db.construct_search_bindings(args, pl_columns)
 
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     query = f"""SELECT
         *
     FROM {args.table}
     WHERE 1=1
         and COALESCE(time_deleted,0) = 0
```

### Comparing `xklb-1.27.3/xklb/subtitle.py` & `xklb-1.27.4/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/tabs_actions.py` & `xklb-1.27.4/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/tabs_extract.py` & `xklb-1.27.4/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/tube_backend.py` & `xklb-1.27.4/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/tube_extract.py` & `xklb-1.27.4/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/utils.py` & `xklb-1.27.4/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/__init__.py` & `xklb-1.27.4/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/bigdirs.py` & `xklb-1.27.4/xklb/scripts/bigdirs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+from pathlib import Path
 from typing import Dict, List
 
 from tabulate import tabulate
 
 from xklb import db, utils
 from xklb.utils import log
 
@@ -27,20 +28,27 @@
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
     parser.add_argument(
         "--size",
         "-S",
         action="append",
         help="Only include files of specific sizes (uses the same syntax as fd-find)",
     )
+    parser.add_argument("--include", "-s", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
+    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("database")
-    args = parser.parse_args()
+    parser.add_argument("search", nargs="*")
+    args = parser.parse_intermixed_args()
     args.db = db.connect(args)
 
+    args.include += args.search
+    if args.include == ["."]:
+        args.include = [str(Path().cwd().resolve())]
+
     if args.size:
         args.size = utils.parse_human_to_sql(utils.human_to_bytes, "size", args.size)
 
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
@@ -101,30 +109,37 @@
         elif args.upper is not None and pdict["count"] > args.upper:
             d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def get_table(args) -> List[dict]:
-    columns = args.db["media"].columns_dict
+    m_columns = args.db["media"].columns_dict
+    args.filter_sql = []
+    args.filter_bindings = {}
+
+    if args.size:
+        args.filter_sql.append(" and size IS NOT NULL " + args.size)
+    db.construct_search_bindings(args, m_columns)
 
     media = list(
         args.db.query(
             f"""
         select
             path
             , size
-            {', time_deleted' if 'time_deleted' in columns else ''}
-            {', time_played' if 'time_played' in columns else ''}
-        from media
+            {', time_deleted' if 'time_deleted' in m_columns else ''}
+            {', time_played' if 'time_played' in m_columns else ''}
+        from media m
         where 1=1
-            {'and time_downloaded > 0' if 'time_downloaded' in columns else ''}
-            {args.size if args.size else ''}
+            {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
+            {" ".join(args.filter_sql)}
         order by path
         """,
+            args.filter_bindings,
         ),
     )
     return media
 
 
 def sort_by(args):
     if args.sort_by:
```

### Comparing `xklb-1.27.3/xklb/scripts/christen.py` & `xklb-1.27.4/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/copy_play_counts.py` & `xklb-1.27.4/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/dedupe.py` & `xklb-1.27.4/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/merge_dbs.py` & `xklb-1.27.4/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/merge_online_local.py` & `xklb-1.27.4/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/move_list.py` & `xklb-1.27.4/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/optimize_db.py` & `xklb-1.27.4/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/redownload.py` & `xklb-1.27.4/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/relmv.py` & `xklb-1.27.4/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/scatter.py` & `xklb-1.27.4/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/streaming_tab_loader.py` & `xklb-1.27.4/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/mining/data.py` & `xklb-1.27.4/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/mining/extract_links.py` & `xklb-1.27.4/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/mining/nouns.py` & `xklb-1.27.4/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/mining/pushshift.py` & `xklb-1.27.4/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.27.4/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/assets/kotobago.png` & `xklb-1.27.4/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/.gitignore` & `xklb-1.27.4/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/LICENSE` & `xklb-1.27.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/README.md` & `xklb-1.27.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.27.003)
+    xk media library subcommands (v1.27.004)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.27.3/pyproject.toml` & `xklb-1.27.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.27.3/PKG-INFO` & `xklb-1.27.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.27.3
+Version: 1.27.4
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
-    xk media library subcommands (v1.27.003)
+    xk media library subcommands (v1.27.004)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

