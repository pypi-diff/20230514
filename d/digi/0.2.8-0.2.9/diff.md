# Comparing `tmp/digi-0.2.8.tar.gz` & `tmp/digi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/digi-0.2.8.tar", last modified: Wed Feb 22 19:52:50 2023, max compression
+gzip compressed data, was "dist/digi-0.2.9.tar", last modified: Sun May 14 07:07:34 2023, max compression
```

## Comparing `digi-0.2.8.tar` & `digi-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-02-22 19:52:50.830766 digi-0.2.8/
--rw-r--r--   0 silv       (501) staff       (20)      240 2023-02-22 19:52:50.830652 digi-0.2.8/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)       15 2021-11-22 01:37:05.000000 digi-0.2.8/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-02-22 19:52:50.824777 digi-0.2.8/digi/
--rw-r--r--   0 silv       (501) staff       (20)     1311 2023-01-01 19:29:18.000000 digi-0.2.8/digi/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       99 2022-01-06 05:51:17.000000 digi-0.2.8/digi/__main__.py
--rw-r--r--   0 silv       (501) staff       (20)     1945 2022-07-04 03:17:20.000000 digi-0.2.8/digi/control.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-02-22 19:52:50.828942 digi-0.2.8/digi/data/
--rw-r--r--   0 silv       (501) staff       (20)      650 2022-11-27 06:55:57.000000 digi-0.2.8/digi/data/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      368 2022-11-03 03:39:08.000000 digi-0.2.8/digi/data/flow.py
--rw-r--r--   0 silv       (501) staff       (20)     3841 2022-11-27 06:58:35.000000 digi-0.2.8/digi/data/pool.py
--rw-r--r--   0 silv       (501) staff       (20)     4104 2022-11-16 23:17:19.000000 digi-0.2.8/digi/data/router.py
--rw-r--r--   0 silv       (501) staff       (20)     8308 2022-11-27 20:24:54.000000 digi-0.2.8/digi/data/sync.py
--rw-r--r--   0 silv       (501) staff       (20)     2227 2022-07-19 06:56:57.000000 digi-0.2.8/digi/data/util.py
--rw-r--r--   0 silv       (501) staff       (20)     1566 2022-12-17 15:37:54.000000 digi-0.2.8/digi/data/zed.py
--rw-r--r--   0 silv       (501) staff       (20)     6650 2022-12-17 15:37:54.000000 digi-0.2.8/digi/data/zjson.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-02-22 19:52:50.829169 digi-0.2.8/digi/dbox/
--rw-r--r--   0 silv       (501) staff       (20)     3015 2022-07-06 08:08:50.000000 digi-0.2.8/digi/dbox/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1163 2022-06-12 02:58:57.000000 digi-0.2.8/digi/filter.py
--rw-r--r--   0 silv       (501) staff       (20)       55 2022-01-06 21:37:00.000000 digi-0.2.8/digi/handler.py
--rw-r--r--   0 silv       (501) staff       (20)     4333 2022-08-05 06:10:18.000000 digi-0.2.8/digi/main.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-02-22 19:52:50.829606 digi-0.2.8/digi/message/
--rw-r--r--   0 silv       (501) staff       (20)      385 2023-01-01 19:29:18.000000 digi-0.2.8/digi/message/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1447 2023-01-01 19:29:18.000000 digi-0.2.8/digi/message/mqtt.py
--rw-r--r--   0 silv       (501) staff       (20)    17899 2022-06-12 00:31:50.000000 digi-0.2.8/digi/mount.py
--rw-r--r--   0 silv       (501) staff       (20)     9955 2022-08-04 20:24:18.000000 digi-0.2.8/digi/on.py
--rw-r--r--   0 silv       (501) staff       (20)      657 2022-02-16 01:07:26.000000 digi-0.2.8/digi/processor.py
--rw-r--r--   0 silv       (501) staff       (20)     7679 2022-10-06 04:44:55.000000 digi-0.2.8/digi/reconcile.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-02-22 19:52:50.830386 digi-0.2.8/digi/tests/
--rw-r--r--   0 silv       (501) staff       (20)        0 2021-11-12 04:46:03.000000 digi-0.2.8/digi/tests/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     5928 2021-11-12 04:46:03.000000 digi-0.2.8/digi/tests/test_mount.py
--rw-r--r--   0 silv       (501) staff       (20)      991 2021-11-12 04:46:03.000000 digi-0.2.8/digi/tests/test_processor.py
--rw-r--r--   0 silv       (501) staff       (20)     1949 2021-11-25 21:23:15.000000 digi-0.2.8/digi/tests/test_view.py
--rw-r--r--   0 silv       (501) staff       (20)    14462 2022-12-17 15:37:54.000000 digi-0.2.8/digi/util.py
--rw-r--r--   0 silv       (501) staff       (20)    10038 2022-01-03 00:55:49.000000 digi-0.2.8/digi/view.py
--rw-r--r--   0 silv       (501) staff       (20)     1230 2022-03-16 06:07:22.000000 digi-0.2.8/digi/visual.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-02-22 19:52:50.825941 digi-0.2.8/digi.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      240 2023-02-22 19:52:50.000000 digi-0.2.8/digi.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)      672 2023-02-22 19:52:50.000000 digi-0.2.8/digi.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2023-02-22 19:52:50.000000 digi-0.2.8/digi.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)       73 2023-02-22 19:52:50.000000 digi-0.2.8/digi.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)        5 2023-02-22 19:52:50.000000 digi-0.2.8/digi.egg-info/top_level.txt
--rw-r--r--   0 silv       (501) staff       (20)       38 2023-02-22 19:52:50.830802 digi-0.2.8/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      567 2023-02-22 19:52:29.000000 digi-0.2.8/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-05-14 07:07:34.422194 digi-0.2.9/
+-rw-r--r--   0 silv       (501) staff       (20)      240 2023-05-14 07:07:34.422071 digi-0.2.9/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)       15 2021-11-22 01:37:05.000000 digi-0.2.9/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-05-14 07:07:34.419390 digi-0.2.9/digi/
+-rw-r--r--   0 silv       (501) staff       (20)     1311 2023-01-01 19:29:18.000000 digi-0.2.9/digi/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       99 2022-01-06 05:51:17.000000 digi-0.2.9/digi/__main__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1945 2022-07-04 03:17:20.000000 digi-0.2.9/digi/control.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-05-14 07:07:34.420836 digi-0.2.9/digi/data/
+-rw-r--r--   0 silv       (501) staff       (20)      650 2022-11-27 06:55:57.000000 digi-0.2.9/digi/data/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      472 2023-05-04 22:52:01.000000 digi-0.2.9/digi/data/flow.py
+-rw-r--r--   0 silv       (501) staff       (20)     3721 2023-04-11 21:40:07.000000 digi-0.2.9/digi/data/pool.py
+-rw-r--r--   0 silv       (501) staff       (20)     4997 2023-05-04 22:57:32.000000 digi-0.2.9/digi/data/router.py
+-rw-r--r--   0 silv       (501) staff       (20)     3099 2023-04-09 15:56:13.000000 digi-0.2.9/digi/data/sourcer.py
+-rw-r--r--   0 silv       (501) staff       (20)     8560 2023-04-17 04:52:06.000000 digi-0.2.9/digi/data/sync.py
+-rw-r--r--   0 silv       (501) staff       (20)      312 2023-04-11 21:53:00.000000 digi-0.2.9/digi/data/util.py
+-rw-r--r--   0 silv       (501) staff       (20)     1566 2022-12-17 15:37:54.000000 digi-0.2.9/digi/data/zed.py
+-rw-r--r--   0 silv       (501) staff       (20)     6650 2022-12-17 15:37:54.000000 digi-0.2.9/digi/data/zjson.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-05-14 07:07:34.420946 digi-0.2.9/digi/dbox/
+-rw-r--r--   0 silv       (501) staff       (20)     3015 2022-07-06 08:08:50.000000 digi-0.2.9/digi/dbox/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1163 2022-06-12 02:58:57.000000 digi-0.2.9/digi/filter.py
+-rw-r--r--   0 silv       (501) staff       (20)       55 2022-01-06 21:37:00.000000 digi-0.2.9/digi/handler.py
+-rw-r--r--   0 silv       (501) staff       (20)     4333 2022-08-05 06:10:18.000000 digi-0.2.9/digi/main.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-05-14 07:07:34.421147 digi-0.2.9/digi/message/
+-rw-r--r--   0 silv       (501) staff       (20)      385 2023-01-01 19:29:18.000000 digi-0.2.9/digi/message/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1447 2023-01-01 19:29:18.000000 digi-0.2.9/digi/message/mqtt.py
+-rw-r--r--   0 silv       (501) staff       (20)    17899 2022-06-12 00:31:50.000000 digi-0.2.9/digi/mount.py
+-rw-r--r--   0 silv       (501) staff       (20)     9938 2023-04-08 05:29:35.000000 digi-0.2.9/digi/on.py
+-rw-r--r--   0 silv       (501) staff       (20)      657 2022-02-16 01:07:26.000000 digi-0.2.9/digi/processor.py
+-rw-r--r--   0 silv       (501) staff       (20)     7679 2022-10-06 04:44:55.000000 digi-0.2.9/digi/reconcile.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-05-14 07:07:34.421919 digi-0.2.9/digi/tests/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2021-11-12 04:46:03.000000 digi-0.2.9/digi/tests/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     5928 2021-11-12 04:46:03.000000 digi-0.2.9/digi/tests/test_mount.py
+-rw-r--r--   0 silv       (501) staff       (20)      991 2021-11-12 04:46:03.000000 digi-0.2.9/digi/tests/test_processor.py
+-rw-r--r--   0 silv       (501) staff       (20)     1949 2021-11-25 21:23:15.000000 digi-0.2.9/digi/tests/test_view.py
+-rw-r--r--   0 silv       (501) staff       (20)    14462 2022-12-17 15:37:54.000000 digi-0.2.9/digi/util.py
+-rw-r--r--   0 silv       (501) staff       (20)    10038 2022-01-03 00:55:49.000000 digi-0.2.9/digi/view.py
+-rw-r--r--   0 silv       (501) staff       (20)     1230 2022-03-16 06:07:22.000000 digi-0.2.9/digi/visual.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-05-14 07:07:34.419925 digi-0.2.9/digi.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      240 2023-05-14 07:07:34.000000 digi-0.2.9/digi.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)      693 2023-05-14 07:07:34.000000 digi-0.2.9/digi.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2023-05-14 07:07:34.000000 digi-0.2.9/digi.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)       73 2023-05-14 07:07:34.000000 digi-0.2.9/digi.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)        5 2023-05-14 07:07:34.000000 digi-0.2.9/digi.egg-info/top_level.txt
+-rw-r--r--   0 silv       (501) staff       (20)       38 2023-05-14 07:07:34.422231 digi-0.2.9/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      400 2023-05-14 07:05:55.000000 digi-0.2.9/setup.py
```

### Comparing `digi-0.2.8/digi/__init__.py` & `digi-0.2.9/digi/__init__.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/control.py` & `digi-0.2.9/digi/control.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/data/__init__.py` & `digi-0.2.9/digi/data/__init__.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/data/pool.py` & `digi-0.2.9/digi/data/pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 import json
 import threading
-import datetime
 from abc import ABC, abstractmethod
 from typing import List, Callable
 
 import digi
 from digi.data import logger, zjson
 from digi.data import sync
 from digi.data import router
+from digi.data import util
 
 
 class Pool(ABC):
     @abstractmethod
     def __init__(self, name: str):
         self.name = name
         self.lock = threading.Lock()
@@ -21,35 +21,26 @@
     def load(self, objects: List[dict]):
         raise NotImplementedError
 
     @abstractmethod
     def query(self, query: str):
         raise NotImplementedError
 
-    @abstractmethod
-    def watch(self, once: Callable, *,
-              branch: str = "main"):
-        raise NotImplementedError
-
-    @abstractmethod
-    def create_branch_if_not_exist(self, query: str):
-        raise NotImplementedError
-
 
 class ZedPool(Pool):
     def __init__(self, name):
         super().__init__(name)
         self.client = digi.data.lake
 
     def load(self, objects: List[dict], *,
              branch="main",
              encoding="zjson",
              same_type=False):
         # update event and processing time
-        now = datetime.datetime.now()
+        now = util.now()
         if encoding == "zjson":
             for o in objects:
                 # event_ts will be attached at the first
                 # data router if does exist from the source
                 if "event_ts" not in o:
                     o["event_ts"] = o.get("ts", now)
                 o["ts"] = now
@@ -70,40 +61,43 @@
             meta = json.dumps({f"{digi.name}": zjson.encode_datetime(now)})
             self.client.load(self.name, data,
                              branch_name=branch,
                              commit_author=digi.name,
                              meta=meta)
             # TBD load from digi also commits source ts in meta
         except Exception as e:
-            digi.logger.warning(f"unable to load "
-                                f"{data} to {self.name}: {e}")
+            logger.warning(f"unable to load "
+                           f"{data} to {self.name}: {e}")
         finally:
             self.lock.release()
 
     def query(self, query: str):
         if query != "":
             query = f"| {query}"
         query = f"from {self.name} {query}"
         return self.client.query(query)
 
-    def watch(self, fn: Callable, *,
+    def watch(self, fn: Callable,
+              branch: str = "main",
+              *,
               in_flow: str = "",
               eoio: bool = True,
               ):
         """Watch changes of the main pool and run UDF."""
-        source = f"{self.name}@main"
+        source = f"{self.name}@{branch}"
         return sync.Watch(fn,
                           sources=[source],
                           eoio=eoio,
                           in_flow=in_flow)
 
     def create_branch_if_not_exist(self, branch: str):
         if not self.client.branch_exist(self.name, branch):
             self.client.create_branch(self.name, branch)
             self.load([router.Egress.INIT], branch=branch)
+            logger.info(f"load {router.Egress.INIT} to {self.name}@{branch}")
 
 
 def pool_name(g, v, r, n, ns):
     _, _, _ = g, v, r
     if ns == "default":
         return f"{n}"
     else:
```

### Comparing `digi-0.2.8/digi/data/router.py` & `digi-0.2.9/digi/data/router.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import digi
 import digi.data.sync as sync
 import digi.data.util as util
-from digi.data import logger, zed
+import digi.data.sourcer as sourcer
+from digi.data import logger, zed, util
 from digi.data import flow as flow_lib
 
 """
 A router contains a collection of pipelets organized as ingresses and egresses.
 Each pipelet is implemented as a digi.data.sync.Sync object that copies and ETL
 data between a source data pool and a destination data pool. 
 """
 
+
 class Router:
     def __init__(self):
         self.ingress = Ingress()
         self.egress = Egress()
 
 
 class Ingress:
@@ -22,104 +24,118 @@
 
     def start(self):
         for name, _sync in self._syncs.items():
             _sync.start()
             logger.info(f"started ingress sync {name} "
                         f"with query: {_sync.query_str}")
 
+    def stop(self):
+        for _, _sync in self._syncs.items():
+            _sync.stop()
+
     def update(self, config: dict):
         self._syncs = dict()
 
         for name, ig in config.items():
             if ig.get("pause", False):
                 continue
 
+            # resolve sources
             sources = list()
-            flow, flow_agg = ig.get("flow", ""), \
-                             ig.get("flow_agg", "")
-            for s in ig.get("source", []):
-                sources += util.parse_source(s)
-            for s in ig.get("sources", []):
-                sources += util.parse_source(s)
+            source_quantifiers = set(ig.get("source", []) + ig.get("sources", []))
+            use_sourcer = ig.get("use_sourcer", False)
 
-            # TBD deduplicate sources
+            # concat and dedup sources
+            for s in source_quantifiers:
+                sources += sourcer.resolve(s, use_sourcer)
+
+            logger.info(f"router: resolved {source_quantifiers} to {sources} "
+                        f"for ingress {name}")
             if len(sources) == 0:
                 continue
 
+            # TBD add support for expressing ingress and egress type on the model
+            # and the optional ingress-egress compatibility check in type.py
+
+            # compile dataflow
+            flow, flow_agg = ig.get("flow", ""), \
+                             ig.get("flow_agg", "")
             if flow_agg == "":
                 _out_flow = flow_lib.refresh_ts
             else:
                 _out_flow = f"{flow_agg} | {flow_lib.refresh_ts}"
 
+            # TBD add support for external pipelet
+            # TBD disambiguate sync updates at fine-grained level
+            # so that skip_history won't skip upon the config changes
+            # or mount changes that don't affect this sync
             _sync = sync.Sync(
                 sources=sources,
                 in_flow=flow,
                 out_flow=_out_flow,
                 dest=digi.pool.name,
                 eoio=ig.get("eoio", True),
                 patch_source=ig.get("patch_source", False),
                 client=zed.Client(),
                 owner=digi.name,
+                min_ts=util.now() if ig.get("skip_history", False) else util.min_time()
             )
             self._syncs[name] = _sync
 
-    def stop(self):
-        for _, _sync in self._syncs.items():
-            _sync.stop()
-
     def restart(self, config: dict):
         self.stop()
         self.update(config=config)
         self.start()
 
-    @staticmethod
-    def _any_source():
-        # TBD fetch all sources - digi and egresses
-        # for digis that are mounted
-        raise NotImplementedError
-
 
 class Egress:
     INIT = {"__meta": "init"}
 
     def __init__(self):
         self._syncs = dict()
 
     def start(self):
         for name, _sync in self._syncs.items():
             _sync.start()
             logger.info(f"started egress sync {name} "
                         f"with query:\n{_sync.query_str}")
 
+    def stop(self):
+        for _, _sync in self._syncs.items():
+            _sync.stop()
+
     def update(self, config: dict):
         self._syncs = dict()
 
-        for name, ig in config.items():
-            if ig.get("driver_managed", False) \
-                    or ig.get("pause", False):
+        for name, eg in config.items():
+            if eg.get("driver_managed", False) \
+                    or eg.get("pause", False):
                 continue
 
-            flow = ig.get("flow", "")
+            flow = eg.get("flow", "")
+            out_flow = f"{flow_lib.drop_meta} | {flow_lib.refresh_ts}"
+            if eg.get("de_id", False):
+                out_flow += f"| {flow_lib.de_id}"
+            if eg.get("link", False):
+                out_flow += f"| {flow_lib.link}"
+
+            # TBD support external sources including external lakes
             _sync = sync.Sync(
                 sources=[digi.pool.name],
                 in_flow=flow,
-                out_flow=f"{flow_lib.drop_meta} | {flow_lib.refresh_ts}",
+                out_flow=out_flow,
                 dest=f"{digi.pool.name}@{name}",
-                eoio=ig.get("eoio", True),
+                eoio=eg.get("eoio", True),
                 client=zed.Client(),
                 owner=digi.name,
             )
             self._syncs[name] = _sync
             # TBD garbage collect unused branches
             digi.pool.create_branch_if_not_exist(name)
 
-    def stop(self):
-        for _, _sync in self._syncs.items():
-            _sync.stop()
-
     def restart(self, config: dict):
         self.stop()
         self.update(config=config)
         self.start()
 
 
 @digi.on.mount
```

### Comparing `digi-0.2.8/digi/data/sync.py` & `digi-0.2.9/digi/data/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-import datetime
+from datetime import datetime, timezone
 import threading
 import typing
 import requests
 import json
 import yaml
 from collections import defaultdict
 
@@ -26,14 +26,15 @@
                  *,
                  poll_interval: float = -1,  # sec, <0: use push
                  eoio: bool = True,  # exactly-once in-order
                  patch_source: bool = False,
                  owner: str = "sync",  # commit author
                  lake_url: str = default_lake_url,
                  client: zed.Client = None,
+                 min_ts: datetime = datetime.min.replace(tzinfo=timezone.utc),
                  ):
         assert len(sources) > 0 and dest != ""
         self.sources = self._normalize(sources)
         self.dest = self._normalize_one(dest)
         self.in_flow = in_flow  # TBD multi-in_flow
         self.out_flow = out_flow
         self.poll_interval = poll_interval
@@ -42,14 +43,15 @@
         # if eoio enabled, the sync agent will
         # process only those records that contain
         # a 'ts' field; XXX assume pool key is ts
         self.eoio = eoio
         self.client = zed.Client(base_url=lake_url) if client is None else client
         self.source_ts = self._fetch_source_ts()  # track {source: max(ts)}
         self.source_pool_ids = self._fetch_source_pool_ids()
+        self.min_ts = min_ts  # min ts to sync
         self.source_set = set(self.sources)
         self.query_str = self._make_query()
 
         threading.Thread.__init__(self)
         self._stop_flag = threading.Event()
 
     def run(self):
@@ -82,15 +84,15 @@
                 if max_ts is None:
                     raise Exception(f"no ts found in records from {source}")
                 if source not in self.source_ts:
                     self.source_ts[source] = max_ts
                 else:
                     self.source_ts[source] = max(max_ts, self.source_ts[source])
             else:
-                self.source_ts[source] = datetime.datetime.min
+                self.source_ts[source] = self.min_ts
         return records
 
     def load(self, records: list):
         records = "\n".join(zjson.encode(records))
         dest_pool, dest_branch = self._denormalize_one(self.dest)
         self.client.load(
             dest_pool, records,
@@ -119,15 +121,15 @@
         while not self._stop_flag.is_set():
             self.once()
             time.sleep(self.poll_interval)
 
     def _make_query(self) -> str:
         in_str = "from (\n"
         for source in self.sources:
-            cur_ts = self.source_ts.get(source, datetime.datetime.min)
+            cur_ts = max(self.source_ts.get(source, self.min_ts), self.min_ts)
             filter_flow = f"ts > {zjson.encode_datetime(cur_ts)} |" \
                 if self.eoio else ""
             patch_source_flow = f"put from := '{source}' |" \
                 if self.patch_source else ""
             in_str += f"pool {source} => {filter_flow} {patch_source_flow} fork (" \
                       f"=> select max(ts) as max_ts | put __from := '{source}' " \
                       f"=> {'pass' if self.in_flow == '' else self.in_flow})"
@@ -152,14 +154,15 @@
                       f"select branch.name as branch," \
                       f"branch.commit as commit |" \
                       f"commit > 0x{'0' * 40}"
         if branch not in set(
                 r["branch"] for r in self.client.query(branch_flow)
         ):
             return source_ts
+
         meta_flow = f"from {self.dest}:log | " \
                     f"typeof(this)==<Commit> | " \
                     f"over meta | " \
                     f"max(cast(value, <time>)) by key | " \
                     f"rename max_ts:=max"
         for r in self.client.query(meta_flow):
             source_ts[r["key"][0]] = r["max_ts"]
@@ -204,26 +207,29 @@
         return pool, branch
 
 
 class Watch(Sync):
     """A destination-less sync that runs a UDF in once()."""
 
     def __init__(self, fn: typing.Callable,
-                 source_ts=None, *args, **kwargs):
+                 source_ts=None,
+                 min_ts=datetime.min.replace(tzinfo=timezone.utc),
+                 *args, **kwargs):
         self.fn = fn
         self.source_ts = source_ts
+        self.min_ts = min_ts
 
         super().__init__(dest="none", *args, **kwargs)
 
     def once(self):
         self.fn(self.read())
 
     def _fetch_source_ts(self) -> dict:
         if self.source_ts is None:
-            return defaultdict(lambda: datetime.datetime.min)
+            return defaultdict(lambda: self.min_ts)
         else:
             return self.source_ts
 
 
 def from_config(path: str) -> Sync:
     with open(path) as f:
         config = yaml.load(f, Loader=yaml.FullLoader)
```

### Comparing `digi-0.2.8/digi/data/util.py` & `digi-0.2.9/digi/data/sourcer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,84 @@
 import typing
 import inflection
+import requests
+
 import digi
 
+default_sourcer_url = "http://sourcer:7534/resolve"
+
+
+def resolve(source, use_sourcer=False):
+    if use_sourcer:
+        return resolve_by_sourcer(source, url=default_sourcer_url)
+    else:
+        return resolve_by_mount(source)
+
+
+def resolve_by_sourcer(source, url):
+    try:
+        # {source_lake_url, sources, success}
+        resp = requests.get(url,
+                            json={"source_quantifier": source},
+                            headers={"Content-Type": "application/json"}).json()
 
-# Each digi can be a data source that has egress attributes.
-# Each egress attribute maps to a data pool branch, e.g., l1@main.
-# A source is uniquely identified by its group, version, kind,
-# name, namespace, and the egress ID/name. The source attribute
-# is parsed with the following rules:
-# - If all attributes are given, a single egress branch is identified.
-# - If the egress ID is omitted, default to main branch at the source pool.
-# - If the name is omitted, default to all sources with of same kind mounted
-#   to the destination.
-# - If the group / version / kind is omitted, default to the destination's
-#   corresponding attribute.
-#   - XXX self-reference is allowed with ingress pointing to the
-#     destination itself
-# TBD add tests
-def parse_source(source: typing.Union[dict, str], *,
-                 exist_only: bool = True) -> typing.List[str]:
+        if resp["success"]:
+            digi.logger.info(f"Resolved {source}")
+            return resp["sources"]
+    except:
+        raise Exception(f"Sourcer unable to resolve {source}")
+
+
+def resolve_by_mount(source: typing.Union[dict, str], *,
+                     exist_only: bool = True) -> typing.List[str]:
     """
     Return the list of egress pool@branch given source attributes.
+    Each digi can be a data source that has egress attributes.
+    Each egress attribute maps to a data pool branch, e.g., l1@main.
+    A source is uniquely identified by its group, version, kind,
+    name, namespace, and the egress ID/name. The source attribute
+    is parsed with the following rules:
+    - If all attributes are given, a single egress branch is identified.
+    - If the egress ID is omitted, default to main branch at the source pool.
+    - If the name is omitted, default to all sources with of same kind mounted
+      to the destination.
+    - If the group / version / kind is omitted, default to the destination's
+    corresponding attribute.
     """
     if isinstance(source, dict):
-        branch = source.get("egress", "main")
-        # XXX assume name is a unique id to digi and ignore namespace
+        egress = source.get("egress", "main")
         if "name" in source:
-            return [f"{source['name']}@{branch}"]
+            return [f"{source['name']}@{egress}"]
         else:
-            group = source.get("group", digi.group)
-            version = source.get("version", digi.version)
-            kind = source.get("kind", digi.kind)
+            g = source.get("group", digi.group)
+            v = source.get("version", digi.version)
+            k = source.get("kind", digi.kind)
+
     elif isinstance(source, str):
         parts = source.split("@")
-        branch = parts[1] if len(parts) > 1 else "main"
-        if "kind:" not in parts[0]:
-            return [f"{parts[0]}@{branch}"]
+        kind_or_name, egress = parts[0], parts[1] if len(parts) > 1 else "main"
+        if kind_or_name.startswith("kind:"):  # this is a direct reference
+            # format: kind:g/v/k@main or kind:k@main;
+            # k <-> r can be used interchangeably
+            kind = kind_or_name[5:]  # remove "kind:"
+            g, v, k = digi.util.parse_kind(kind)
         else:
-            # kind:g/v/k@main or kind:k@main; k <-> r
-            kind = parts[0].lstrip("kind:")
-            group, version, kind = digi.util.parse_kind(kind)
+            return [f"{kind_or_name}@{egress}"]
     else:
         raise NotImplementedError
 
-    if kind == "any":
+    if k == "any":
         mounts = digi.model.get_mount(any=True)
     else:
-        mounts = digi.model.get_mount(group, version, inflection.pluralize(kind))
-    pools = [digi.util.trim_default_namespace(name) for name in mounts.keys()] \
-        if mounts else []
-
-    return [f"{pool}@{branch}"
-            for pool in pools if not exist_only
-            or digi.data.lake.branch_exist(pool, branch)]
+        mounts = digi.model.get_mount(g, v, inflection.pluralize(k))
+
+    if mounts is None:
+        return []
+    digi.logger.info(f"sourcer: detect matching mounts {mounts} for {source}")
+
+    pools = [digi.util.trim_default_namespace(name) for name in mounts.keys()]
+    digi.logger.info(f"sourcer: resolve {source} to {pools} by mount")
+
+    # TBD support multiple egresses
+    # TBD disallow self-reference
+    return [f"{pool}@{egress}" for pool in pools
+            if not exist_only or digi.data.lake.branch_exist(pool, egress)]
```

### Comparing `digi-0.2.8/digi/data/zed.py` & `digi-0.2.9/digi/data/zed.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/data/zjson.py` & `digi-0.2.9/digi/data/zjson.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/dbox/__init__.py` & `digi-0.2.9/digi/dbox/__init__.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/filter.py` & `digi-0.2.9/digi/filter.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/main.py` & `digi-0.2.9/digi/main.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/message/mqtt.py` & `digi-0.2.9/digi/message/mqtt.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/mount.py` & `digi-0.2.9/digi/mount.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/on.py` & `digi-0.2.9/digi/on.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
         def stop(self):
             self.watch.stop()
 
     # @pool
     if len(args) == 1 and len(kwargs) == 0 and callable(args[0]):
         digi.rc.add_data_watch(
             name=watch_name(args[0]),
-            watch=DelayedWatch(args[0], *args, **kwargs),
+            watch=DelayedWatch(args[0]),
         )
         return args[0]
 
     # @pool(*args, **kwargs)
     def decorator(fn):
         digi.rc.add_data_watch(
             name=watch_name(fn),
```

### Comparing `digi-0.2.8/digi/processor.py` & `digi-0.2.9/digi/processor.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/reconcile.py` & `digi-0.2.9/digi/reconcile.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/tests/test_mount.py` & `digi-0.2.9/digi/tests/test_mount.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/tests/test_processor.py` & `digi-0.2.9/digi/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/tests/test_view.py` & `digi-0.2.9/digi/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/util.py` & `digi-0.2.9/digi/util.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/view.py` & `digi-0.2.9/digi/view.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi/visual.py` & `digi-0.2.9/digi/visual.py`

 * *Files identical despite different names*

### Comparing `digi-0.2.8/digi.egg-info/SOURCES.txt` & `digi-0.2.9/digi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 digi.egg-info/dependency_links.txt
 digi.egg-info/requires.txt
 digi.egg-info/top_level.txt
 digi/data/__init__.py
 digi/data/flow.py
 digi/data/pool.py
 digi/data/router.py
+digi/data/sourcer.py
 digi/data/sync.py
 digi/data/util.py
 digi/data/zed.py
 digi/data/zjson.py
 digi/dbox/__init__.py
 digi/message/__init__.py
 digi/message/mqtt.py
```

