# Comparing `tmp/gandai-1.1.6.tar.gz` & `tmp/gandai-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.1.6.tar", last modified: Sun May 14 02:15:01 2023, max compression
+gzip compressed data, was "gandai-1.1.7.tar", last modified: Sun May 14 18:15:28 2023, max compression
```

## Comparing `gandai-1.1.6.tar` & `gandai-1.1.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.195051 gandai-1.1.6/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.6/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-14 02:15:01.194928 gandai-1.1.6/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.189261 gandai-1.1.6/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.6/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.192817 gandai-1.1.6/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.6/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.6/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.6/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4064 2023-05-14 00:47:34.000000 gandai-1.1.6/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.6/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.6/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5068 2023-05-12 19:30:40.000000 gandai-1.1.6/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6064 2023-05-12 19:41:17.000000 gandai-1.1.6/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16436 2023-05-14 01:24:41.000000 gandai-1.1.6/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.6/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7849 2023-05-12 19:25:42.000000 gandai-1.1.6/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1699 2023-05-13 19:58:43.000000 gandai-1.1.6/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1583 2023-05-14 00:47:07.000000 gandai-1.1.6/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.6/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     3286 2023-05-12 19:30:37.000000 gandai-1.1.6/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.193842 gandai-1.1.6/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.6/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.194320 gandai-1.1.6/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.1.6/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6097 2023-05-13 21:29:04.000000 gandai-1.1.6/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.6/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1680 2023-05-13 21:28:48.000000 gandai-1.1.6/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3043 2023-05-14 01:40:03.000000 gandai-1.1.6/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.194663 gandai-1.1.6/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)     2815 2023-05-13 19:15:16.000000 gandai-1.1.6/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2592 2023-05-12 19:41:16.000000 gandai-1.1.6/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)     8697 2023-05-14 01:24:23.000000 gandai-1.1.6/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     5442 2023-05-14 02:14:15.000000 gandai-1.1.6/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.189798 gandai-1.1.6/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-14 02:15:01.000000 gandai-1.1.6/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1015 2023-05-14 02:15:01.000000 gandai-1.1.6/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-14 02:15:01.000000 gandai-1.1.6/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-14 02:15:01.000000 gandai-1.1.6/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-14 02:14:55.000000 gandai-1.1.6/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-14 02:15:01.195082 gandai-1.1.6/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.6/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.373960 gandai-1.1.7/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.7/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-14 18:15:28.373853 gandai-1.1.7/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.371071 gandai-1.1.7/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.7/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.372893 gandai-1.1.7/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.7/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.7/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.7/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4064 2023-05-14 00:47:34.000000 gandai-1.1.7/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.7/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.7/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5068 2023-05-12 19:30:40.000000 gandai-1.1.7/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6137 2023-05-14 03:30:02.000000 gandai-1.1.7/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    16436 2023-05-14 01:24:41.000000 gandai-1.1.7/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.7/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7849 2023-05-12 19:25:42.000000 gandai-1.1.7/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1699 2023-05-13 19:58:43.000000 gandai-1.1.7/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1583 2023-05-14 00:47:07.000000 gandai-1.1.7/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.7/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     3295 2023-05-14 18:08:29.000000 gandai-1.1.7/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.373338 gandai-1.1.7/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.7/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.373572 gandai-1.1.7/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.1.7/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6424 2023-05-14 03:30:02.000000 gandai-1.1.7/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.7/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1626 2023-05-14 03:24:47.000000 gandai-1.1.7/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3257 2023-05-14 17:36:57.000000 gandai-1.1.7/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.373704 gandai-1.1.7/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)     2843 2023-05-14 17:45:11.000000 gandai-1.1.7/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2642 2023-05-14 03:28:36.000000 gandai-1.1.7/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)     8697 2023-05-14 01:24:23.000000 gandai-1.1.7/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     5442 2023-05-14 02:14:15.000000 gandai-1.1.7/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.371575 gandai-1.1.7/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-14 18:15:28.000000 gandai-1.1.7/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1015 2023-05-14 18:15:28.000000 gandai-1.1.7/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-14 18:15:28.000000 gandai-1.1.7/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-14 18:15:28.000000 gandai-1.1.7/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2023-05-14 18:09:10.000000 gandai-1.1.7/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-14 18:15:28.373990 gandai-1.1.7/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.7/setup.py
```

### Comparing `gandai-1.1.6/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/models.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5c965e64 (Fri May 12 19:41:16 2023 UTC)
-files sz: 2592
+moddate:  0x64556064 (Sun May 14 03:28:36 2023 UTC)
+files sz: 2642
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
@@ -88,151 +88,151 @@
                132 CALL                     2
    
     15         142 PRECALL                  0
                146 CALL                     0
    
     16         156 STORE_NAME              11 (Company)
    
-    24         158 PUSH_NULL
+    25         158 PUSH_NULL
                160 LOAD_BUILD_CLASS
-               162 LOAD_CONST              10 (<code object EventType, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 24>)
+               162 LOAD_CONST              10 (<code object EventType, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 25>)
                164 MAKE_FUNCTION            0
                166 LOAD_CONST              11 ('EventType')
                168 LOAD_NAME               12 (str)
                170 LOAD_NAME                4 (Enum)
                172 PRECALL                  4
                176 CALL                     4
                186 STORE_NAME              13 (EventType)
    
-    35         188 LOAD_NAME                8 (dataclass)
+    36         188 LOAD_NAME                8 (dataclass)
    
-    36         190 PUSH_NULL
+    37         190 PUSH_NULL
                192 LOAD_BUILD_CLASS
-               194 LOAD_CONST              12 (<code object Event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 35>)
+               194 LOAD_CONST              12 (<code object Event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 36>)
                196 MAKE_FUNCTION            0
                198 LOAD_CONST              13 ('Event')
                200 PRECALL                  2
                204 CALL                     2
    
-    35         214 PRECALL                  0
+    36         214 PRECALL                  0
                218 CALL                     0
    
-    36         228 STORE_NAME              14 (Event)
+    37         228 STORE_NAME              14 (Event)
    
-    47         230 LOAD_NAME                8 (dataclass)
+    48         230 LOAD_NAME                8 (dataclass)
    
-    48         232 PUSH_NULL
+    49         232 PUSH_NULL
                234 LOAD_BUILD_CLASS
-               236 LOAD_CONST              14 (<code object Comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 47>)
+               236 LOAD_CONST              14 (<code object Comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 48>)
                238 MAKE_FUNCTION            0
                240 LOAD_CONST              15 ('Comment')
                242 LOAD_NAME               14 (Event)
                244 PRECALL                  3
                248 CALL                     3
    
-    47         258 PRECALL                  0
+    48         258 PRECALL                  0
                262 CALL                     0
    
-    48         272 STORE_NAME              15 (Comment)
+    49         272 STORE_NAME              15 (Comment)
    
-    53         274 LOAD_NAME                8 (dataclass)
+    54         274 LOAD_NAME                8 (dataclass)
    
-    54         276 PUSH_NULL
+    55         276 PUSH_NULL
                278 LOAD_BUILD_CLASS
-               280 LOAD_CONST              16 (<code object Rating, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 53>)
+               280 LOAD_CONST              16 (<code object Rating, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 54>)
                282 MAKE_FUNCTION            0
                284 LOAD_CONST              17 ('Rating')
                286 LOAD_NAME               14 (Event)
                288 PRECALL                  3
                292 CALL                     3
    
-    53         302 PRECALL                  0
+    54         302 PRECALL                  0
                306 CALL                     0
    
-    54         316 STORE_NAME              16 (Rating)
+    55         316 STORE_NAME              16 (Rating)
    
-    58         318 LOAD_NAME                8 (dataclass)
+    59         318 LOAD_NAME                8 (dataclass)
    
-    59         320 PUSH_NULL
+    60         320 PUSH_NULL
                322 LOAD_BUILD_CLASS
-               324 LOAD_CONST              18 (<code object Checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 58>)
+               324 LOAD_CONST              18 (<code object Checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 59>)
                326 MAKE_FUNCTION            0
                328 LOAD_CONST              19 ('Checkpoint')
                330 PRECALL                  2
                334 CALL                     2
    
-    58         344 PRECALL                  0
+    59         344 PRECALL                  0
                348 CALL                     0
    
-    59         358 STORE_NAME              17 (Checkpoint)
+    60         358 STORE_NAME              17 (Checkpoint)
    
-    65         360 PUSH_NULL
+    66         360 PUSH_NULL
                362 LOAD_NAME                8 (dataclass)
                364 LOAD_CONST               6 (True)
                366 KW_NAMES                 7
                368 PRECALL                  1
                372 CALL                     1
    
-    66         382 PUSH_NULL
+    67         382 PUSH_NULL
                384 LOAD_BUILD_CLASS
-               386 LOAD_CONST              20 (<code object Target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 65>)
+               386 LOAD_CONST              20 (<code object Target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 66>)
                388 MAKE_FUNCTION            0
                390 LOAD_CONST              21 ('Target')
                392 PRECALL                  2
                396 CALL                     2
    
-    65         406 PRECALL                  0
+    66         406 PRECALL                  0
                410 CALL                     0
    
-    66         420 STORE_NAME              18 (Target)
+    67         420 STORE_NAME              18 (Target)
    
-    77         422 LOAD_NAME                8 (dataclass)
+    78         422 LOAD_NAME                8 (dataclass)
    
-    78         424 PUSH_NULL
+    79         424 PUSH_NULL
                426 LOAD_BUILD_CLASS
-               428 LOAD_CONST              22 (<code object Criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 77>)
+               428 LOAD_CONST              22 (<code object Criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 78>)
                430 MAKE_FUNCTION            0
                432 LOAD_CONST              23 ('Criteria')
                434 PRECALL                  2
                438 CALL                     2
    
-    77         448 PRECALL                  0
+    78         448 PRECALL                  0
                452 CALL                     0
    
-    78         462 STORE_NAME              19 (Criteria)
+    79         462 STORE_NAME              19 (Criteria)
    
-    93         464 LOAD_NAME                8 (dataclass)
+    94         464 LOAD_NAME                8 (dataclass)
    
-    94         466 PUSH_NULL
+    95         466 PUSH_NULL
                468 LOAD_BUILD_CLASS
-               470 LOAD_CONST              24 (<code object Search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 93>)
+               470 LOAD_CONST              24 (<code object Search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 94>)
                472 MAKE_FUNCTION            0
                474 LOAD_CONST              25 ('Search')
                476 PRECALL                  2
                480 CALL                     2
    
-    93         490 PRECALL                  0
+    94         490 PRECALL                  0
                494 CALL                     0
    
-    94         504 STORE_NAME              20 (Search)
+    95         504 STORE_NAME              20 (Search)
    
-   108         506 LOAD_NAME                8 (dataclass)
+   109         506 LOAD_NAME                8 (dataclass)
    
-   109         508 PUSH_NULL
+   110         508 PUSH_NULL
                510 LOAD_BUILD_CLASS
-               512 LOAD_CONST              26 (<code object Sort, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 108>)
+               512 LOAD_CONST              26 (<code object Sort, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 109>)
                514 MAKE_FUNCTION            0
                516 LOAD_CONST              27 ('Sort')
                518 PRECALL                  2
                522 CALL                     2
    
-   108         532 PRECALL                  0
+   109         532 PRECALL                  0
                536 CALL                     0
    
-   109         546 STORE_NAME              21 (Sort)
+   110         546 STORE_NAME              21 (Sort)
                548 LOAD_CONST              28 (None)
                550 RETURN_VALUE
    consts
       0
       ('List', 'Optional')
       ('Enum', 'auto')
       ('asdict', 'dataclass', 'field')
@@ -290,15 +290,17 @@
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c00000064025a05650665
             0319000000000000000000650464033c00000064025a0765066503190000
             00000000000000650464043c000000020065086509ac05a6010000ab0100
             000000000000005a0a6509650464063c000000020065086402ac07a60100
-            00ab0100000000000000005a0b650c650464083c00000064025300
+            00ab0100000000000000005a0b650c650464083c000000020065086402ac
+            07a6010000ab0100000000000000005a0d650c650464093c000000640253
+            00
           15           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Company')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -344,96 +346,109 @@
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_NAME              11 (id)
                      132 LOAD_NAME               12 (int)
                      134 LOAD_NAME                4 (__annotations__)
                      136 LOAD_CONST               8 ('id')
                      138 STORE_SUBSCR
-                     142 LOAD_CONST               2 (None)
-                     144 RETURN_VALUE
+         
+          22         142 PUSH_NULL
+                     144 LOAD_NAME                8 (field)
+                     146 LOAD_CONST               2 (None)
+                     148 KW_NAMES                 7
+                     150 PRECALL                  1
+                     154 CALL                     1
+                     164 STORE_NAME              13 (uid)
+                     166 LOAD_NAME               12 (int)
+                     168 LOAD_NAME                4 (__annotations__)
+                     170 LOAD_CONST               9 ('uid')
+                     172 STORE_SUBSCR
+                     176 LOAD_CONST               2 (None)
+                     178 RETURN_VALUE
          consts
             'Company'
             'domain'
             None
             'name'
             'description'
             ('default_factory',)
             'meta'
             ('default',)
             'id'
-         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'name', 'Optional', 'description', 'field', 'dict', 'meta', 'id', 'int')
+            'uid'
+         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'name', 'Optional', 'description', 'field', 'dict', 'meta', 'id', 'int', 'uid')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Company'
          firstlineno 15
-         lnotab 0x0c020a011a011a012201
+         lnotab 0x0c020a011a011a0122012201
       'Company'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0202006503a6000000ab0000000000000000005a
             0402006503a6000000ab0000000000000000005a0502006503a6000000ab
             0000000000000000005a0602006503a6000000ab0000000000000000005a
             0702006503a6000000ab0000000000000000005a0802006503a6000000ab
             0000000000000000005a0902006503a6000000ab0000000000000000005a
             0a02006503a6000000ab0000000000000000005a0b64015300
-          24           0 RESUME                   0
+          25           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('EventType')
                        8 STORE_NAME               2 (__qualname__)
          
-          25          10 PUSH_NULL
+          26          10 PUSH_NULL
                       12 LOAD_NAME                3 (auto)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_NAME               4 (CREATE)
          
-          26          30 PUSH_NULL
+          27          30 PUSH_NULL
                       32 LOAD_NAME                3 (auto)
                       34 PRECALL                  0
                       38 CALL                     0
                       48 STORE_NAME               5 (ADVANCE)
          
-          27          50 PUSH_NULL
+          28          50 PUSH_NULL
                       52 LOAD_NAME                3 (auto)
                       54 PRECALL                  0
                       58 CALL                     0
                       68 STORE_NAME               6 (VALIDATE)
          
-          28          70 PUSH_NULL
+          29          70 PUSH_NULL
                       72 LOAD_NAME                3 (auto)
                       74 PRECALL                  0
                       78 CALL                     0
                       88 STORE_NAME               7 (SEND)
          
-          29          90 PUSH_NULL
+          30          90 PUSH_NULL
                       92 LOAD_NAME                3 (auto)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 STORE_NAME               8 (CLIENT_ACCEPT)
          
-          30         110 PUSH_NULL
+          31         110 PUSH_NULL
                      112 LOAD_NAME                3 (auto)
                      114 PRECALL                  0
                      118 CALL                     0
                      128 STORE_NAME               9 (CONFLICT)
          
-          31         130 PUSH_NULL
+          32         130 PUSH_NULL
                      132 LOAD_NAME                3 (auto)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 STORE_NAME              10 (REJECT)
          
-          32         150 PUSH_NULL
+          33         150 PUSH_NULL
                      152 LOAD_NAME                3 (auto)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 STORE_NAME              11 (CRITERIA)
                      170 LOAD_CONST               1 (None)
                      172 RETURN_VALUE
          consts
@@ -441,70 +456,70 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'auto', 'CREATE', 'ADVANCE', 'VALIDATE', 'SEND', 'CLIENT_ACCEPT', 'CONFLICT', 'REJECT', 'CRITERIA')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'EventType'
-         firstlineno 24
+         firstlineno 25
          lnotab 0x0a011401140114011401140114011401
       'EventType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c00000065056506190000
             00000000000000650464023c0000006506650464033c0000006506650464
             043c000000020065076508ac05a6010000ab0100000000000000005a0965
             08650464063c000000020065076407ac08a6010000ab0100000000000000
             005a0a6503650464093c00000064075300
-          35           0 RESUME                   0
+          36           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Event')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          38          12 LOAD_NAME                3 (int)
+          39          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('search_uid')
                       18 STORE_SUBSCR
          
-          39          22 LOAD_NAME                5 (Optional)
+          40          22 LOAD_NAME                5 (Optional)
                       24 LOAD_NAME                6 (str)
                       26 BINARY_SUBSCR
                       36 LOAD_NAME                4 (__annotations__)
                       38 LOAD_CONST               2 ('domain')
                       40 STORE_SUBSCR
          
-          40          44 LOAD_NAME                6 (str)
+          41          44 LOAD_NAME                6 (str)
                       46 LOAD_NAME                4 (__annotations__)
                       48 LOAD_CONST               3 ('actor_key')
                       50 STORE_SUBSCR
          
-          41          54 LOAD_NAME                6 (str)
+          42          54 LOAD_NAME                6 (str)
                       56 LOAD_NAME                4 (__annotations__)
                       58 LOAD_CONST               4 ('type')
                       60 STORE_SUBSCR
          
-          42          64 PUSH_NULL
+          43          64 PUSH_NULL
                       66 LOAD_NAME                7 (field)
                       68 LOAD_NAME                8 (dict)
                       70 KW_NAMES                 5
                       72 PRECALL                  1
                       76 CALL                     1
                       86 STORE_NAME               9 (data)
                       88 LOAD_NAME                8 (dict)
                       90 LOAD_NAME                4 (__annotations__)
                       92 LOAD_CONST               6 ('data')
                       94 STORE_SUBSCR
          
-          43          98 PUSH_NULL
+          44          98 PUSH_NULL
                      100 LOAD_NAME                7 (field)
                      102 LOAD_CONST               7 (None)
                      104 KW_NAMES                 8
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_NAME              10 (id)
                      122 LOAD_NAME                3 (int)
@@ -526,30 +541,30 @@
             'id'
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'Optional', 'str', 'field', 'dict', 'data', 'id')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Event'
-         firstlineno 35
+         firstlineno 36
          lnotab 0x0c030a0116010a010a012201
       'Event'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          47           0 RESUME                   0
+          48           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Comment')
                        8 STORE_NAME               2 (__qualname__)
          
-          49          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 49>)
+          50          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 50>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__post_init__)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'Comment'
             code
@@ -557,17 +572,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000640119
                   000000000000000000740400000000000000000000a6020000ab02000000
                   000000000073024a00820164005300
-                49           0 RESUME                   0
+                50           0 RESUME                   0
                
-                50           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                51           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (data)
                             26 LOAD_CONST               1 ('comment')
                             28 BINARY_SUBSCR
                             38 LOAD_GLOBAL              4 (str)
                             50 PRECALL                  2
                             54 CALL                     2
@@ -581,39 +596,39 @@
                   'comment'
                names      ('isinstance', 'data', 'str')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '__post_init__'
-               firstlineno 49
+               firstlineno 50
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Comment'
-         firstlineno 47
+         firstlineno 48
          lnotab 0x0a02
       'Comment'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          53           0 RESUME                   0
+          54           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Rating')
                        8 STORE_NAME               2 (__qualname__)
          
-          55          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 55>)
+          56          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 56>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__post_init__)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'Rating'
             code
@@ -621,17 +636,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000640119
                   000000000000000000740400000000000000000000a6020000ab02000000
                   000000000073024a00820164005300
-                55           0 RESUME                   0
+                56           0 RESUME                   0
                
-                56           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                57           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (data)
                             26 LOAD_CONST               1 ('rating')
                             28 BINARY_SUBSCR
                             38 LOAD_GLOBAL              4 (int)
                             50 PRECALL                  2
                             54 CALL                     2
@@ -645,48 +660,48 @@
                   'rating'
                names      ('isinstance', 'data', 'int')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '__post_init__'
-               firstlineno 55
+               firstlineno 56
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Rating'
-         firstlineno 53
+         firstlineno 54
          lnotab 0x0a02
       'Rating'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c000000020065056402ac
             03a6010000ab0100000000000000005a066503650464043c000000640253
             00
-          58           0 RESUME                   0
+          59           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Checkpoint')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          61          12 LOAD_NAME                3 (int)
+          62          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('event_id')
                       18 STORE_SUBSCR
          
-          62          22 PUSH_NULL
+          63          22 PUSH_NULL
                       24 LOAD_NAME                5 (field)
                       26 LOAD_CONST               2 (None)
                       28 KW_NAMES                 3
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               6 (id)
                       46 LOAD_NAME                3 (int)
@@ -703,70 +718,70 @@
             'id'
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'field', 'id')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Checkpoint'
-         firstlineno 58
+         firstlineno 59
          lnotab 0x0c030a01
       'Checkpoint'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006503650464023c
             0000006505650464033c0000006503650464043c0000006506650464053c
             0000006503650464063c0000006505650464073c0000006507650464083c
             00000064095300
-          65           0 RESUME                   0
+          66           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Target')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          67          12 LOAD_NAME                3 (str)
+          68          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('domain')
                       18 STORE_SUBSCR
          
-          68          22 LOAD_NAME                3 (str)
+          69          22 LOAD_NAME                3 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('name')
                       28 STORE_SUBSCR
          
-          69          32 LOAD_NAME                5 (int)
+          70          32 LOAD_NAME                5 (int)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('search_id')
                       38 STORE_SUBSCR
          
-          70          42 LOAD_NAME                3 (str)
+          71          42 LOAD_NAME                3 (str)
                       44 LOAD_NAME                4 (__annotations__)
                       46 LOAD_CONST               4 ('description')
                       48 STORE_SUBSCR
          
-          71          52 LOAD_NAME                6 (List)
+          72          52 LOAD_NAME                6 (List)
                       54 LOAD_NAME                4 (__annotations__)
                       56 LOAD_CONST               5 ('event')
                       58 STORE_SUBSCR
          
-          72          62 LOAD_NAME                3 (str)
+          73          62 LOAD_NAME                3 (str)
                       64 LOAD_NAME                4 (__annotations__)
                       66 LOAD_CONST               6 ('last_event_type')
                       68 STORE_SUBSCR
          
-          73          72 LOAD_NAME                5 (int)
+          74          72 LOAD_NAME                5 (int)
                       74 LOAD_NAME                4 (__annotations__)
                       76 LOAD_CONST               7 ('last_rating')
                       78 STORE_SUBSCR
          
-          74          82 LOAD_NAME                7 (dict)
+          75          82 LOAD_NAME                7 (dict)
                       84 LOAD_NAME                4 (__annotations__)
                       86 LOAD_CONST               8 ('meta')
                       88 STORE_SUBSCR
                       92 LOAD_CONST               9 (None)
                       94 RETURN_VALUE
          consts
             'Target'
@@ -781,91 +796,91 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'int', 'List', 'dict')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Target'
-         firstlineno 65
+         firstlineno 66
          lnotab 0x0c020a010a010a010a010a010a010a01
       'Target'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006505650464023c
             0000006505650464033c0000006506650464043c0000006506650464053c
             0000006506650464063c0000006506650464073c0000006506650464083c
             0000006506650464093c00000065066504640a3c00000065036504640b3c
             00000065036504640c3c000000640d5300
-          77           0 RESUME                   0
+          78           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Criteria')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          79          12 LOAD_NAME                3 (int)
+          80          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('search_id')
                       18 STORE_SUBSCR
          
-          80          22 LOAD_NAME                5 (str)
+          81          22 LOAD_NAME                5 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('type')
                       28 STORE_SUBSCR
          
-          81          32 LOAD_NAME                5 (str)
+          82          32 LOAD_NAME                5 (str)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('prompt')
                       38 STORE_SUBSCR
          
-          82          42 LOAD_NAME                6 (list)
+          83          42 LOAD_NAME                6 (list)
                       44 LOAD_NAME                4 (__annotations__)
                       46 LOAD_CONST               4 ('rating')
                       48 STORE_SUBSCR
          
-          83          52 LOAD_NAME                6 (list)
+          84          52 LOAD_NAME                6 (list)
                       54 LOAD_NAME                4 (__annotations__)
                       56 LOAD_CONST               5 ('employees_range')
                       58 STORE_SUBSCR
          
-          84          62 LOAD_NAME                6 (list)
+          85          62 LOAD_NAME                6 (list)
                       64 LOAD_NAME                4 (__annotations__)
                       66 LOAD_CONST               6 ('country')
                       68 STORE_SUBSCR
          
-          85          72 LOAD_NAME                6 (list)
+          86          72 LOAD_NAME                6 (list)
                       74 LOAD_NAME                4 (__annotations__)
                       76 LOAD_CONST               7 ('state')
                       78 STORE_SUBSCR
          
-          86          82 LOAD_NAME                6 (list)
+          87          82 LOAD_NAME                6 (list)
                       84 LOAD_NAME                4 (__annotations__)
                       86 LOAD_CONST               8 ('ownership')
                       88 STORE_SUBSCR
          
-          87          92 LOAD_NAME                6 (list)
+          88          92 LOAD_NAME                6 (list)
                       94 LOAD_NAME                4 (__annotations__)
                       96 LOAD_CONST               9 ('product')
                       98 STORE_SUBSCR
          
-          88         102 LOAD_NAME                6 (list)
+          89         102 LOAD_NAME                6 (list)
                      104 LOAD_NAME                4 (__annotations__)
                      106 LOAD_CONST              10 ('services')
                      108 STORE_SUBSCR
          
-          89         112 LOAD_NAME                3 (int)
+          90         112 LOAD_NAME                3 (int)
                      114 LOAD_NAME                4 (__annotations__)
                      116 LOAD_CONST              11 ('updated')
                      118 STORE_SUBSCR
          
-          90         122 LOAD_NAME                3 (int)
+          91         122 LOAD_NAME                3 (int)
                      124 LOAD_NAME                4 (__annotations__)
                      126 LOAD_CONST              12 ('actor_id')
                      128 STORE_SUBSCR
                      132 LOAD_CONST              13 (None)
                      134 RETURN_VALUE
          consts
             'Criteria'
@@ -884,15 +899,15 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'list')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Criteria'
-         firstlineno 77
+         firstlineno 78
          lnotab 0x0c020a010a010a010a010a010a010a010a010a010a010a01
       'Criteria'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
@@ -901,85 +916,85 @@
             0000006505650464033c000000020065066507ac04a6010000ab01000000
             00000000005a086507650464053c000000020065066507ac04a6010000ab
             0100000000000000005a096507650464063c000000020065066507ac04a6
             010000ab0100000000000000005a0a6507650464073c0000000200650665
             07ac04a6010000ab0100000000000000005a0b6507650464083c00000002
             0065066409ac0aa6010000ab0100000000000000005a0c65036504640b3c
             00000064095300
-          93           0 RESUME                   0
+          94           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Search')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          96          12 LOAD_NAME                3 (int)
+          97          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('uid')
                       18 STORE_SUBSCR
          
-          97          22 LOAD_NAME                5 (str)
+          98          22 LOAD_NAME                5 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('client_domain')
                       28 STORE_SUBSCR
          
-          98          32 LOAD_NAME                5 (str)
+          99          32 LOAD_NAME                5 (str)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('label')
                       38 STORE_SUBSCR
          
-          99          42 PUSH_NULL
+         100          42 PUSH_NULL
                       44 LOAD_NAME                6 (field)
                       46 LOAD_NAME                7 (dict)
                       48 KW_NAMES                 4
                       50 PRECALL                  1
                       54 CALL                     1
                       64 STORE_NAME               8 (meta)
                       66 LOAD_NAME                7 (dict)
                       68 LOAD_NAME                4 (__annotations__)
                       70 LOAD_CONST               5 ('meta')
                       72 STORE_SUBSCR
          
-         100          76 PUSH_NULL
+         101          76 PUSH_NULL
                       78 LOAD_NAME                6 (field)
                       80 LOAD_NAME                7 (dict)
                       82 KW_NAMES                 4
                       84 PRECALL                  1
                       88 CALL                     1
                       98 STORE_NAME               9 (inclusion)
                      100 LOAD_NAME                7 (dict)
                      102 LOAD_NAME                4 (__annotations__)
                      104 LOAD_CONST               6 ('inclusion')
                      106 STORE_SUBSCR
          
-         101         110 PUSH_NULL
+         102         110 PUSH_NULL
                      112 LOAD_NAME                6 (field)
                      114 LOAD_NAME                7 (dict)
                      116 KW_NAMES                 4
                      118 PRECALL                  1
                      122 CALL                     1
                      132 STORE_NAME              10 (exclusion)
                      134 LOAD_NAME                7 (dict)
                      136 LOAD_NAME                4 (__annotations__)
                      138 LOAD_CONST               7 ('exclusion')
                      140 STORE_SUBSCR
          
-         102         144 PUSH_NULL
+         103         144 PUSH_NULL
                      146 LOAD_NAME                6 (field)
                      148 LOAD_NAME                7 (dict)
                      150 KW_NAMES                 4
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_NAME              11 (sort)
                      168 LOAD_NAME                7 (dict)
                      170 LOAD_NAME                4 (__annotations__)
                      172 LOAD_CONST               8 ('sort')
                      174 STORE_SUBSCR
          
-         103         178 PUSH_NULL
+         104         178 PUSH_NULL
                      180 LOAD_NAME                6 (field)
                      182 LOAD_CONST               9 (None)
                      184 KW_NAMES                10
                      186 PRECALL                  1
                      190 CALL                     1
                      200 STORE_NAME              12 (id)
                      202 LOAD_NAME                3 (int)
@@ -1003,48 +1018,48 @@
             'id'
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'inclusion', 'exclusion', 'sort', 'id')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Search'
-         firstlineno 93
+         firstlineno 94
          lnotab 0x0c030a010a010a012201220122012201
       'Search'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a02550067006401a2015a036402640367025a0465
             05650664043c0000006505650664053c00000064065300
-         108           0 RESUME                   0
+         109           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Sort')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         110          12 BUILD_LIST               0
+         111          12 BUILD_LIST               0
                       14 LOAD_CONST               1 (('employee_count', 'rating', 'state', 'country', 'year_founded', 'name'))
                       16 LIST_EXTEND              1
                       18 STORE_NAME               3 (FIELDS)
          
-         111          20 LOAD_CONST               2 ('asc')
+         112          20 LOAD_CONST               2 ('asc')
                       22 LOAD_CONST               3 ('desc')
                       24 BUILD_LIST               2
                       26 STORE_NAME               4 (ORDERS)
          
-         113          28 LOAD_NAME                5 (str)
+         114          28 LOAD_NAME                5 (str)
                       30 LOAD_NAME                6 (__annotations__)
                       32 LOAD_CONST               4 ('field')
                       34 STORE_SUBSCR
          
-         114          38 LOAD_NAME                5 (str)
+         115          38 LOAD_NAME                5 (str)
                       40 LOAD_NAME                6 (__annotations__)
                       42 LOAD_CONST               5 ('order')
                       44 STORE_SUBSCR
                       48 LOAD_CONST               6 (None)
                       50 RETURN_VALUE
          consts
             'Sort'
@@ -1056,23 +1071,23 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'FIELDS', 'ORDERS', 'str', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Sort'
-         firstlineno 108
+         firstlineno 109
          lnotab 0x0c02080108020a01
       'Sort'
       None
    names      ('typing', 'List', 'Optional', 'enum', 'Enum', 'auto', 'dataclasses', 'asdict', 'dataclass', 'field', 'Actor', 'Company', 'str', 'EventType', 'Event', 'Comment', 'Rating', 'Checkpoint', 'Target', 'Criteria', 'Search', 'Sort')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201100110011402020118ff0e010209160118ff0e0102081e0b02
+      0x00ff0201100110011402020118ff0e010209160118ff0e0102091e0b02
       0118ff0e01020b02011aff0e01020502011aff0e010204020118ff0e0102
       06160118ff0e01020b020118ff0e01020f020118ff0e01020e020118ff0e
       01
```

### Comparing `gandai-1.1.6/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.1.7/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/auth.py` & `gandai-1.1.7/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/datastore.py` & `gandai-1.1.7/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/db.py` & `gandai-1.1.7/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/main.py` & `gandai-1.1.7/gandai/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         resp = grata.enrich(company.domain)
         if resp.get("status") == 404:
             print(f"{company} not found")
         else:
             print(resp)
             company.name = resp.get("name")
             company.description = resp.get("description")
-            company.meta = company.meta | resp  # merge
+            company.meta = {**company.meta, **resp} # merge 3.5+
             query.update_company(company)
 
     elif e.type == "validate":
         search = query.find_search_by_uid(search_uid)
         _insert_companies(
             companies=grata.find_similar(domain=e.domain, search=search), 
             existing_domains=query.target(search_uid=search_uid)["domain"].tolist()
```

### Comparing `gandai-1.1.6/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.1.7/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x1c016064 (Sat May 13 21:29:00 2023 UTC)
-files sz: 2988
+moddate:  0x8a546064 (Sun May 14 03:24:58 2023 UTC)
+files sz: 3252
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c045a04640064036c055a06640a640565066a07000000000000000066
-      02640684055a08640b640884015a09640984005a0a64035300
+      036c045a04640064036c055a060900640c640565066a0700000000000000
+      006602640684055a08640d640884015a09640984005a0a640a84005a0b65
+      0c640b6b0200000000720c0200650ba6000000ab00000000000000000001
+      006403530064035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('query',))
                  6 IMPORT_NAME              0 (gandai)
                  8 IMPORT_FROM              1 (query)
                 10 STORE_NAME               1 (query)
@@ -32,142 +34,165 @@
                 32 STORE_NAME               4 (re)
    
      5          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               3 (None)
                 38 IMPORT_NAME              5 (pandas)
                 40 STORE_NAME               6 (pd)
    
-     8          42 LOAD_CONST              10 (('data/company.xlsx',))
-                44 LOAD_CONST               5 ('return')
-                46 LOAD_NAME                6 (pd)
-                48 LOAD_ATTR                7 (DataFrame)
-                58 BUILD_TUPLE              2
-                60 LOAD_CONST               6 (<code object dealcloud_company_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 8>)
-                62 MAKE_FUNCTION            5 (defaults, annotations)
-                64 STORE_NAME               8 (dealcloud_company_query)
-   
-    30          66 LOAD_CONST              11 (('data/Engagement_05132023.xlsx',))
-                68 LOAD_CONST               8 (<code object dealcloud_engagements, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 30>)
-                70 MAKE_FUNCTION            1 (defaults)
-                72 STORE_NAME               9 (dealcloud_engagements)
-   
-    51          74 LOAD_CONST               9 (<code object migrate_engagements, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 51>)
-                76 MAKE_FUNCTION            0
-                78 STORE_NAME              10 (migrate_engagements)
-                80 LOAD_CONST               3 (None)
-                82 RETURN_VALUE
+     9          42 NOP
+   
+     8          44 LOAD_CONST              12 (('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx',))
+                46 LOAD_CONST               5 ('return')
+   
+    10          48 LOAD_NAME                6 (pd)
+                50 LOAD_ATTR                7 (DataFrame)
+   
+     8          60 BUILD_TUPLE              2
+                62 LOAD_CONST               6 (<code object dealcloud_company_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 8>)
+                64 MAKE_FUNCTION            5 (defaults, annotations)
+                66 STORE_NAME               8 (dealcloud_company_query)
+   
+    33          68 LOAD_CONST              13 (('data/Engagement_05132023.xlsx',))
+                70 LOAD_CONST               8 (<code object dealcloud_engagements, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 33>)
+                72 MAKE_FUNCTION            1 (defaults)
+                74 STORE_NAME               9 (dealcloud_engagements)
+   
+    54          76 LOAD_CONST               9 (<code object migrate_engagements, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 54>)
+                78 MAKE_FUNCTION            0
+                80 STORE_NAME              10 (migrate_engagements)
+   
+    88          82 LOAD_CONST              10 (<code object main, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 88>)
+                84 MAKE_FUNCTION            0
+                86 STORE_NAME              11 (main)
+   
+    92          88 LOAD_NAME               12 (__name__)
+                90 LOAD_CONST              11 ('__main__')
+                92 COMPARE_OP               2 (==)
+                98 POP_JUMP_FORWARD_IF_FALSE    12 (to 124)
+   
+    93         100 PUSH_NULL
+               102 LOAD_NAME               11 (main)
+               104 PRECALL                  0
+               108 CALL                     0
+               118 POP_TOP
+               120 LOAD_CONST               3 (None)
+               122 RETURN_VALUE
+   
+    92     >>  124 LOAD_CONST               3 (None)
+               126 RETURN_VALUE
    consts
       0
       ('query',)
       ('Search',)
       None
-      'data/company.xlsx'
+      '/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx'
       'return'
       code
          argcount  : 1
          nlocals   : 3
-         stacksize : 4
+         stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             00010064027402000000000000000000006602640384047d017405000000
             000000000000006a0300000000000000007c00a6010000ab010000000000
             0000007d02640484007c026a0400000000000000004400a6000000ab0000
             000000000000007c025f04000000000000000064057c026a040000000000
             000000760073024a0082017c02640619000000000000000000a005000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a00600000000000000000000000000000000000000007c01a6010000ab
             0100000000000000007c0264073c0000007c026408190000000000000000
             00a0050000000000000000000000000000000000000000a6000000ab0000
             00000000000000a006000000000000000000000000000000000000000064
             098400a6010000ab0100000000000000007c0264083c0000007c02a00700
-            00000000000000000000000000000000000000640a640b6901ac0ca60100
-            00ab0100000000000000007d027c025300
+            00000000000000000000000000000000000000640a640b640c9c02ac0da6
+            010000ab0100000000000000007d027c025300
            8           0 RESUME                   0
          
-           9           2 LOAD_GLOBAL              1 (NULL + print)
+          11           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('dealcloud_company_query')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-          10          32 LOAD_CONST               2 ('return')
+          13          32 LOAD_CONST               2 ('return')
                       34 LOAD_GLOBAL              2 (str)
                       46 BUILD_TUPLE              2
-                      48 LOAD_CONST               3 (<code object _get_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 10>)
+                      48 LOAD_CONST               3 (<code object _get_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 13>)
                       50 MAKE_FUNCTION            4 (annotations)
                       52 STORE_FAST               1 (_get_domain)
          
-          14          54 LOAD_GLOBAL              5 (NULL + pd)
+          17          54 LOAD_GLOBAL              5 (NULL + pd)
                       66 LOAD_ATTR                3 (read_excel)
                       76 LOAD_FAST                0 (fp)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (df)
          
-          15          94 LOAD_CONST               4 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 15>)
+          18          94 LOAD_CONST               4 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 18>)
                       96 MAKE_FUNCTION            0
                       98 LOAD_FAST                2 (df)
                      100 LOAD_ATTR                4 (columns)
                      110 GET_ITER
                      112 PRECALL                  0
                      116 CALL                     0
                      126 LOAD_FAST                2 (df)
                      128 STORE_ATTR               4 (columns)
          
-          16         138 LOAD_CONST               5 ('dealcloud_id')
+          19         138 LOAD_CONST               5 ('dealcloud_id')
                      140 LOAD_FAST                2 (df)
                      142 LOAD_ATTR                4 (columns)
                      152 CONTAINS_OP              0
                      154 POP_JUMP_FORWARD_IF_TRUE     2 (to 160)
                      156 LOAD_ASSERTION_ERROR
                      158 RAISE_VARARGS            1
          
-          17     >>  160 LOAD_FAST                2 (df)
+          20     >>  160 LOAD_FAST                2 (df)
                      162 LOAD_CONST               6 ('website')
                      164 BINARY_SUBSCR
                      174 LOAD_METHOD              5 (dropna)
                      196 PRECALL                  0
                      200 CALL                     0
                      210 LOAD_METHOD              6 (apply)
                      232 LOAD_FAST                1 (_get_domain)
                      234 PRECALL                  1
                      238 CALL                     1
                      248 LOAD_FAST                2 (df)
                      250 LOAD_CONST               7 ('domain')
                      252 STORE_SUBSCR
          
-          19         256 LOAD_FAST                2 (df)
+          22         256 LOAD_FAST                2 (df)
                      258 LOAD_CONST               8 ('days_since_contact')
                      260 BINARY_SUBSCR
                      270 LOAD_METHOD              5 (dropna)
                      292 PRECALL                  0
                      296 CALL                     0
                      306 LOAD_METHOD              6 (apply)
-                     328 LOAD_CONST               9 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 19>)
+                     328 LOAD_CONST               9 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 22>)
                      330 MAKE_FUNCTION            0
                      332 PRECALL                  1
                      336 CALL                     1
          
-          18         346 LOAD_FAST                2 (df)
+          21         346 LOAD_FAST                2 (df)
                      348 LOAD_CONST               8 ('days_since_contact')
                      350 STORE_SUBSCR
          
-          21         354 LOAD_FAST                2 (df)
+          24         354 LOAD_FAST                2 (df)
                      356 LOAD_METHOD              7 (rename)
-                     378 LOAD_CONST              10 ('company_name')
-                     380 LOAD_CONST              11 ('name')
-                     382 BUILD_MAP                1
-                     384 KW_NAMES                12
-                     386 PRECALL                  1
-                     390 CALL                     1
-                     400 STORE_FAST               2 (df)
+                     378 LOAD_CONST              10 ('name')
+                     380 LOAD_CONST              11 ('description')
+                     382 LOAD_CONST              12 (('company_name', 'business_description'))
+                     384 BUILD_CONST_KEY_MAP      2
+                     386 KW_NAMES                13
+                     388 PRECALL                  1
+                     392 CALL                     1
+                     402 STORE_FAST               2 (df)
          
-          27         402 LOAD_FAST                2 (df)
-                     404 RETURN_VALUE
+          30         404 LOAD_FAST                2 (df)
+                     406 RETURN_VALUE
          consts
             None
             'dealcloud_company_query'
             'return'
             code
                argcount  : 1
                nlocals   : 1
@@ -177,17 +202,17 @@
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02a6020000ab020000000000000000a00000000000000000000000000000
                   0000000000000064036402a6020000ab020000000000000000a000000000
                   000000000000000000000000000000000064046402a6020000ab02000000
                   00000000007d007c00a00100000000000000000000000000000000000000
                   006405a6010000ab01000000000000000064061900000000000000000053
                   00
-                10           0 RESUME                   0
+                13           0 RESUME                   0
                
-                11           2 LOAD_FAST                0 (url)
+                14           2 LOAD_FAST                0 (url)
                              4 LOAD_METHOD              0 (replace)
                             26 LOAD_CONST               1 ('http://')
                             28 LOAD_CONST               2 ('')
                             30 PRECALL                  2
                             34 CALL                     2
                             44 LOAD_METHOD              0 (replace)
                             66 LOAD_CONST               3 ('https://')
@@ -197,15 +222,15 @@
                             84 LOAD_METHOD              0 (replace)
                            106 LOAD_CONST               4 ('www.')
                            108 LOAD_CONST               2 ('')
                            110 PRECALL                  2
                            114 CALL                     2
                            124 STORE_FAST               0 (url)
                
-                12         126 LOAD_FAST                0 (url)
+                15         126 LOAD_FAST                0 (url)
                            128 LOAD_METHOD              1 (split)
                            150 LOAD_CONST               5 ('/')
                            152 PRECALL                  1
                            156 CALL                     1
                            166 LOAD_CONST               6 (0)
                            168 BINARY_SUBSCR
                            178 RETURN_VALUE
@@ -219,28 +244,28 @@
                   0
                names      ('replace', 'split')
                varnames   ('url',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '_get_domain'
-               firstlineno 10
+               firstlineno 13
                lnotab 0x02017c01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d3e7d017c01a000000000000000000000000000000000
                   000000000064006401a6020000ab020000000000000000a0000000000000
                   00000000000000000000000000000064026403a6020000ab020000000000
                   000000a0010000000000000000000000000000000000000000a6000000ab
                   00000000000000000091028c3f5300
-                15           0 RESUME                   0
+                18           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                62 (to 132)
                              8 STORE_FAST               1 (col)
                             10 LOAD_FAST                1 (col)
                             12 LOAD_METHOD              0 (replace)
                             34 LOAD_CONST               0 (' ')
@@ -265,30 +290,30 @@
                   ''
                names      ('replace', 'lower')
                varnames   ('.0', 'col')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '<listcomp>'
-               firstlineno 15
+               firstlineno 18
                lnotab 0x
             'dealcloud_id'
             'website'
             'domain'
             'days_since_contact'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 19
                code
                   0x97007401000000000000000000007403000000000000000000006a0200
                   0000000000000064017c00a6020000ab0200000000000000006402190000
                   00000000000000a6010000ab0100000000000000005300
-                19           0 RESUME                   0
+                22           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + int)
                             14 LOAD_GLOBAL              3 (NULL + re)
                             26 LOAD_ATTR                2 (findall)
                             36 LOAD_CONST               1 ('\\d+')
                             38 LOAD_FAST                0 (x)
                             40 PRECALL                  2
                             44 CALL                     2
@@ -303,27 +328,28 @@
                   0
                names      ('int', 're', 'findall')
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '<lambda>'
-               firstlineno 19
+               firstlineno 22
                lnotab 0x
-            'company_name'
             'name'
+            'description'
+            ('company_name', 'business_description')
             ('columns',)
          names      ('print', 'str', 'pd', 'read_excel', 'columns', 'dropna', 'apply', 'rename')
          varnames   ('fp', '_get_domain', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
          name       'dealcloud_company_query'
          firstlineno 8
-         lnotab 0x02011e01160428012c01160160025aff08033006
+         lnotab 0x02031e02160428012c01160160025aff08033206
       'data/Engagement_05132023.xlsx'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -347,174 +373,174 @@
             00000000000000a00b000000000000000000000000000000000000000067
             00640da201a6010000ab0100000000000000000f00190000000000000000
             00a00c0000000000000000000000000000000000000000640eac0fa60100
             00ab0100000000000000007d017c017c0164051900000000000000000064
             106b000000000019000000000000000000a00c0000000000000000000000
             000000000000000000640eac0fa6010000ab0100000000000000007d017c
             015300
-          30           0 RESUME                   0
+          33           0 RESUME                   0
          
-          31           2 LOAD_GLOBAL              1 (NULL + pd)
+          34           2 LOAD_GLOBAL              1 (NULL + pd)
                       14 LOAD_ATTR                1 (read_excel)
                       24 LOAD_FAST                0 (fp)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               1 (df)
          
-          32          42 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 32>)
+          35          42 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 35>)
                       44 MAKE_FUNCTION            0
                       46 LOAD_FAST                1 (df)
                       48 LOAD_ATTR                2 (columns)
                       58 GET_ITER
                       60 PRECALL                  0
                       64 CALL                     0
                       74 LOAD_FAST                1 (df)
                       76 STORE_ATTR               2 (columns)
          
-          33          86 LOAD_FAST                1 (df)
+          36          86 LOAD_FAST                1 (df)
                       88 LOAD_CONST               2 ('dealcloud_id')
                       90 BINARY_SUBSCR
                      100 LOAD_METHOD              3 (astype)
                      122 LOAD_GLOBAL              8 (str)
                      134 PRECALL                  1
                      138 CALL                     1
                      148 LOAD_FAST                1 (df)
                      150 LOAD_CONST               2 ('dealcloud_id')
                      152 STORE_SUBSCR
          
-          34         156 LOAD_CONST               2 ('dealcloud_id')
+          37         156 LOAD_CONST               2 ('dealcloud_id')
                      158 LOAD_FAST                1 (df)
                      160 LOAD_ATTR                2 (columns)
                      170 CONTAINS_OP              0
                      172 POP_JUMP_FORWARD_IF_TRUE     2 (to 178)
                      174 LOAD_ASSERTION_ERROR
                      176 RAISE_VARARGS            1
          
-          35     >>  178 LOAD_GLOBAL              1 (NULL + pd)
+          38     >>  178 LOAD_GLOBAL              1 (NULL + pd)
                      190 LOAD_ATTR                5 (to_datetime)
                      200 LOAD_CONST               3 ('today')
                      202 PRECALL                  1
                      206 CALL                     1
                      216 STORE_FAST               2 (today)
          
-          36         218 LOAD_FAST                2 (today)
+          39         218 LOAD_FAST                2 (today)
                      220 LOAD_GLOBAL              1 (NULL + pd)
                      232 LOAD_ATTR                5 (to_datetime)
                      242 LOAD_FAST                1 (df)
                      244 LOAD_CONST               4 ('modified_date')
                      246 BINARY_SUBSCR
                      256 PRECALL                  1
                      260 CALL                     1
                      270 BINARY_OP               10 (-)
                      274 LOAD_ATTR                6 (dt)
                      284 LOAD_ATTR                7 (days)
                      294 LOAD_FAST                1 (df)
                      296 LOAD_CONST               5 ('modified_days_ago')
                      298 STORE_SUBSCR
          
-          37         302 LOAD_CONST               6 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 37>)
+          40         302 LOAD_CONST               6 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 40>)
                      304 MAKE_FUNCTION            0
                      306 LOAD_FAST                1 (df)
                      308 LOAD_ATTR                2 (columns)
                      318 GET_ITER
                      320 PRECALL                  0
                      324 CALL                     0
                      334 STORE_FAST               3 (date_cols)
          
-          38         336 LOAD_FAST                3 (date_cols)
+          41         336 LOAD_FAST                3 (date_cols)
                      338 GET_ITER
                  >>  340 FOR_ITER                33 (to 408)
                      342 STORE_FAST               4 (col)
          
-          39         344 LOAD_FAST                1 (df)
+          42         344 LOAD_FAST                1 (df)
                      346 LOAD_FAST                4 (col)
                      348 BINARY_SUBSCR
                      358 LOAD_METHOD              8 (apply)
-                     380 LOAD_CONST               7 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 39>)
+                     380 LOAD_CONST               7 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 42>)
                      382 MAKE_FUNCTION            0
                      384 PRECALL                  1
                      388 CALL                     1
                      398 LOAD_FAST                1 (df)
                      400 LOAD_FAST                4 (col)
                      402 STORE_SUBSCR
                      406 JUMP_BACKWARD           34 (to 340)
          
-          40     >>  408 LOAD_FAST                1 (df)
+          43     >>  408 LOAD_FAST                1 (df)
                      410 LOAD_METHOD              9 (dropna)
                      432 LOAD_CONST               8 ('engagement_name')
                      434 BUILD_LIST               1
                      436 KW_NAMES                 9
                      438 PRECALL                  1
                      442 CALL                     1
                      452 STORE_FAST               1 (df)
          
-          41         454 LOAD_FAST                1 (df)
+          44         454 LOAD_FAST                1 (df)
                      456 LOAD_METHOD             10 (sort_values)
                      478 LOAD_CONST               4 ('modified_date')
                      480 LOAD_CONST              10 (False)
                      482 KW_NAMES                11
                      484 PRECALL                  2
                      488 CALL                     2
                      498 STORE_FAST               1 (df)
          
-          42         500 LOAD_FAST                1 (df)
+          45         500 LOAD_FAST                1 (df)
          
-          43         502 LOAD_FAST                1 (df)
+          46         502 LOAD_FAST                1 (df)
                      504 LOAD_CONST              12 ('status')
                      506 BINARY_SUBSCR
                      516 LOAD_METHOD             11 (isin)
          
-          44         538 BUILD_LIST               0
+          47         538 BUILD_LIST               0
                      540 LOAD_CONST              13 (('Lost Pre-Mandate', 'Completed Engagement', 'Dead Post-Mandate'))
                      542 LIST_EXTEND              1
          
-          43         544 PRECALL                  1
+          46         544 PRECALL                  1
                      548 CALL                     1
                      558 UNARY_INVERT
          
-          42         560 BINARY_SUBSCR
+          45         560 BINARY_SUBSCR
          
-          46         570 LOAD_METHOD             12 (reset_index)
+          49         570 LOAD_METHOD             12 (reset_index)
                      592 LOAD_CONST              14 (True)
                      594 KW_NAMES                15
                      596 PRECALL                  1
                      600 CALL                     1
          
-          42         610 STORE_FAST               1 (df)
+          45         610 STORE_FAST               1 (df)
          
-          47         612 LOAD_FAST                1 (df)
+          50         612 LOAD_FAST                1 (df)
                      614 LOAD_FAST                1 (df)
                      616 LOAD_CONST               5 ('modified_days_ago')
                      618 BINARY_SUBSCR
                      628 LOAD_CONST              16 (365)
                      630 COMPARE_OP               0 (<)
                      636 BINARY_SUBSCR
                      646 LOAD_METHOD             12 (reset_index)
                      668 LOAD_CONST              14 (True)
                      670 KW_NAMES                15
                      672 PRECALL                  1
                      676 CALL                     1
                      686 STORE_FAST               1 (df)
          
-          48         688 LOAD_FAST                1 (df)
+          51         688 LOAD_FAST                1 (df)
                      690 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d3e7d017c01a000000000000000000000000000000000
                   0000000000a6000000ab000000000000000000a001000000000000000000
                   000000000000000000000064006401a6020000ab020000000000000000a0
                   01000000000000000000000000000000000000000064026403a6020000ab
                   02000000000000000091028c3f5300
-                32           0 RESUME                   0
+                35           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                62 (to 132)
                              8 STORE_FAST               1 (col)
                             10 LOAD_FAST                1 (col)
                             12 LOAD_METHOD              0 (lower)
                             34 PRECALL                  0
@@ -539,30 +565,30 @@
                   ''
                names      ('lower', 'replace')
                varnames   ('.0', 'col')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '<listcomp>'
-               firstlineno 32
+               firstlineno 35
                lnotab 0x
             'dealcloud_id'
             'today'
             'modified_date'
             'modified_days_ago'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x970067007c005d197d017c01a000000000000000000000000000000000
                   00000000006400a6010000ab010000000000000000af177c0191028c1a53
                   00
-                37           0 RESUME                   0
+                40           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                25 (to 58)
                              8 STORE_FAST               1 (col)
                             10 LOAD_FAST                1 (col)
                             12 LOAD_METHOD              0 (endswith)
                             34 LOAD_CONST               0 ('_date')
@@ -577,25 +603,25 @@
                   '_date'
                names      ('endswith',)
                varnames   ('.0', 'col')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '<listcomp>'
-               firstlineno 37
+               firstlineno 40
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   00640164028502190000000000000000005300
-                39           0 RESUME                   0
+                42           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + str)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_CONST               1 (0)
                             32 LOAD_CONST               2 (10)
                             34 BUILD_SLICE              2
@@ -607,15 +633,15 @@
                   10
                names      ('str',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '<lambda>'
-               firstlineno 39
+               firstlineno 42
                lnotab 0x
             'engagement_name'
             ('subset',)
             False
             ('ascending',)
             'status'
             ('Lost Pre-Mandate', 'Completed Engagement', 'Dead Post-Mandate')
@@ -624,166 +650,171 @@
             365
          names      ('pd', 'read_excel', 'columns', 'astype', 'str', 'to_datetime', 'dt', 'days', 'apply', 'dropna', 'sort_values', 'isin', 'reset_index')
          varnames   ('fp', 'df', 'today', 'date_cols', 'col')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
          name       'dealcloud_engagements'
-         firstlineno 30
+         firstlineno 33
          lnotab
             0x020128012c0146011601280154012201080140012e012e010201240106
             ff10ff0a0428fc02054c01
       code
          argcount  : 0
          nlocals   : 5
-         stacksize : 10
+         stacksize : 11
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             007d007403000000000000000000006402a6010000ab0100000000000000
             007d017c017c01640319000000000000000000a002000000000000000000
             00000000000000000000007c00640419000000000000000000a6010000ab
             010000000000000000190000000000000000007d027c02a0030000000000
             000000000000000000000000000000640564066901ac07a6010000ab0100
             00000000000000640364066702190000000000000000007d027c00a00400
             000000000000000000000000000000000000007c02640464036408ac09a6
             040000ab0400000000000000007d007c00a0050000000000000000000000
             000000000000000000640aa6010000ab010000000000000000a006000000
             0000000000000000000000000000000000640bac0ca6010000ab01000000
-            000000000044005d5e7d03740f0000000000000000000074110000000000
+            000000000044005d627d03740f0000000000000000000074110000000000
             00000000007c03640d19000000000000000000a6010000ab010000000000
             0000007c036406190000000000000000007c03640e190000000000000000
-            007c03640f670164106411670264129c02ac13a6050000ab050000000000
-            0000007d047413000000000000000000007c04a6010000ab010000000000
-            00000001007415000000000000000000006a0b00000000000000007c04a6
-            010000ab01000000000000000001008c5f64005300
-          51           0 RESUME                   0
+            007c03640f670164106411670264129c026405641364149c02ac15a60600
+            00ab0600000000000000007d047413000000000000000000007c04a60100
+            00ab01000000000000000001007415000000000000000000006a0b000000
+            00000000007c04a6010000ab01000000000000000001008c6364005300
+          54           0 RESUME                   0
          
-          52           2 LOAD_GLOBAL              1 (NULL + dealcloud_engagements)
+          55           2 LOAD_GLOBAL              1 (NULL + dealcloud_engagements)
          
-          53          14 LOAD_CONST               1 ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Engagement_05132023.xlsx')
+          56          14 LOAD_CONST               1 ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Engagement_05132023.xlsx')
          
-          52          16 PRECALL                  1
+          55          16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               0 (engagements)
          
-          55          32 LOAD_GLOBAL              3 (NULL + dealcloud_company_query)
+          58          32 LOAD_GLOBAL              3 (NULL + dealcloud_company_query)
          
-          56          44 LOAD_CONST               2 ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx')
+          59          44 LOAD_CONST               2 ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx')
          
-          55          46 PRECALL                  1
+          58          46 PRECALL                  1
                       50 CALL                     1
                       60 STORE_FAST               1 (companies)
          
-          59          62 LOAD_FAST                1 (companies)
+          62          62 LOAD_FAST                1 (companies)
                       64 LOAD_FAST                1 (companies)
                       66 LOAD_CONST               3 ('name')
                       68 BINARY_SUBSCR
                       78 LOAD_METHOD              2 (isin)
                      100 LOAD_FAST                0 (engagements)
                      102 LOAD_CONST               4 ('client')
                      104 BINARY_SUBSCR
                      114 PRECALL                  1
                      118 CALL                     1
                      128 BINARY_SUBSCR
                      138 STORE_FAST               2 (clients)
          
-          60         140 LOAD_FAST                2 (clients)
+          63         140 LOAD_FAST                2 (clients)
                      142 LOAD_METHOD              3 (rename)
                      164 LOAD_CONST               5 ('domain')
                      166 LOAD_CONST               6 ('client_domain')
                      168 BUILD_MAP                1
                      170 KW_NAMES                 7
                      172 PRECALL                  1
                      176 CALL                     1
          
-          61         186 LOAD_CONST               3 ('name')
+          64         186 LOAD_CONST               3 ('name')
                      188 LOAD_CONST               6 ('client_domain')
                      190 BUILD_LIST               2
          
-          60         192 BINARY_SUBSCR
+          63         192 BINARY_SUBSCR
                      202 STORE_FAST               2 (clients)
          
-          64         204 LOAD_FAST                0 (engagements)
+          67         204 LOAD_FAST                0 (engagements)
                      206 LOAD_METHOD              4 (merge)
          
-          65         228 LOAD_FAST                2 (clients)
+          68         228 LOAD_FAST                2 (clients)
                      230 LOAD_CONST               4 ('client')
                      232 LOAD_CONST               3 ('name')
                      234 LOAD_CONST               8 ('left')
          
-          64         236 KW_NAMES                 9
+          67         236 KW_NAMES                 9
                      238 PRECALL                  4
                      242 CALL                     4
                      252 STORE_FAST               0 (engagements)
          
-          68         254 LOAD_FAST                0 (engagements)
+          71         254 LOAD_FAST                0 (engagements)
                      256 LOAD_METHOD              5 (fillna)
                      278 LOAD_CONST              10 ('')
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_METHOD              6 (to_dict)
                      316 LOAD_CONST              11 ('records')
                      318 KW_NAMES                12
                      320 PRECALL                  1
                      324 CALL                     1
                      334 GET_ITER
-                 >>  336 FOR_ITER                94 (to 526)
+                 >>  336 FOR_ITER                98 (to 534)
                      338 STORE_FAST               3 (engagement)
          
-          69         340 LOAD_GLOBAL             15 (NULL + Search)
+          72         340 LOAD_GLOBAL             15 (NULL + Search)
          
-          70         352 LOAD_GLOBAL             17 (NULL + int)
+          73         352 LOAD_GLOBAL             17 (NULL + int)
                      364 LOAD_FAST                3 (engagement)
                      366 LOAD_CONST              13 ('dealcloud_id')
                      368 BINARY_SUBSCR
                      378 PRECALL                  1
                      382 CALL                     1
          
-          71         392 LOAD_FAST                3 (engagement)
+          74         392 LOAD_FAST                3 (engagement)
                      394 LOAD_CONST               6 ('client_domain')
                      396 BINARY_SUBSCR
          
-          72         406 LOAD_FAST                3 (engagement)
+          75         406 LOAD_FAST                3 (engagement)
                      408 LOAD_CONST              14 ('engagement_name')
                      410 BINARY_SUBSCR
          
-          73         420 LOAD_FAST                3 (engagement)
+          76         420 LOAD_FAST                3 (engagement)
          
-          75         422 LOAD_CONST              15 ('USA')
+          78         422 LOAD_CONST              15 ('USA')
                      424 BUILD_LIST               1
          
-          76         426 LOAD_CONST              16 (10)
+          79         426 LOAD_CONST              16 (10)
                      428 LOAD_CONST              17 (100)
                      430 BUILD_LIST               2
          
-          74         432 LOAD_CONST              18 (('country', 'employees_range'))
+          77         432 LOAD_CONST              18 (('country', 'employees_range'))
                      434 BUILD_CONST_KEY_MAP      2
          
-          69         436 KW_NAMES                19
-                     438 PRECALL                  5
-                     442 CALL                     5
-                     452 STORE_FAST               4 (search)
-         
-          79         454 LOAD_GLOBAL             19 (NULL + print)
-                     466 LOAD_FAST                4 (search)
-                     468 PRECALL                  1
-                     472 CALL                     1
-                     482 POP_TOP
-         
-          80         484 LOAD_GLOBAL             21 (NULL + query)
-                     496 LOAD_ATTR               11 (insert_search)
-                     506 LOAD_FAST                4 (search)
-                     508 PRECALL                  1
-                     512 CALL                     1
-                     522 POP_TOP
-                     524 JUMP_BACKWARD           95 (to 336)
+          81         436 LOAD_CONST               5 ('domain')
+                     438 LOAD_CONST              19 ('desc')
+                     440 LOAD_CONST              20 (('field', 'order'))
+                     442 BUILD_CONST_KEY_MAP      2
+         
+          72         444 KW_NAMES                21
+                     446 PRECALL                  6
+                     450 CALL                     6
+                     460 STORE_FAST               4 (search)
+         
+          83         462 LOAD_GLOBAL             19 (NULL + print)
+                     474 LOAD_FAST                4 (search)
+                     476 PRECALL                  1
+                     480 CALL                     1
+                     490 POP_TOP
+         
+          84         492 LOAD_GLOBAL             21 (NULL + query)
+                     504 LOAD_ATTR               11 (insert_search)
+                     514 LOAD_FAST                4 (search)
+                     516 PRECALL                  1
+                     520 CALL                     1
+                     530 POP_TOP
+                     532 JUMP_BACKWARD           99 (to 336)
          
-          68     >>  526 LOAD_CONST               0 (None)
-                     528 RETURN_VALUE
+          71     >>  534 LOAD_CONST               0 (None)
+                     536 RETURN_VALUE
          consts
             None
             '/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Engagement_05132023.xlsx'
             '/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx'
             'name'
             'client'
             'domain'
@@ -796,28 +827,59 @@
             ('orient',)
             'dealcloud_id'
             'engagement_name'
             'USA'
             10
             100
             ('country', 'employees_range')
-            ('uid', 'client_domain', 'label', 'meta', 'inclusion')
+            'desc'
+            ('field', 'order')
+            ('uid', 'client_domain', 'label', 'meta', 'inclusion', 'sort')
          names      ('dealcloud_engagements', 'dealcloud_company_query', 'isin', 'rename', 'merge', 'fillna', 'to_dict', 'Search', 'int', 'print', 'query', 'insert_search')
          varnames   ('engagements', 'companies', 'clients', 'engagement', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
          name       'migrate_engagements'
-         firstlineno 51
+         firstlineno 54
          lnotab
             0x02010c0102ff10030c0102ff10044e012e0106ff0c04180108ff120456
-            010c0128010e010e010202040106fe04fb120a1e012af4
-      ('data/company.xlsx',)
+            010c0128010e010e010202040106fe040408f7120b1e012af3
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 2
+         flags     : 3
+         code
+            0x9700740100000000000000000000a6000000ab00000000000000000001
+            0064005300
+          88           0 RESUME                   0
+         
+          89           2 LOAD_GLOBAL              1 (NULL + migrate_engagements)
+                      14 PRECALL                  0
+                      18 CALL                     0
+                      28 POP_TOP
+                      30 LOAD_CONST               0 (None)
+                      32 RETURN_VALUE
+         consts
+            None
+         names      ('migrate_engagements',)
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
+         name       'main'
+         firstlineno 88
+         lnotab 0x0201
+      '__main__'
+      ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx',)
       ('data/Engagement_05132023.xlsx',)
-   names      ('gandai', 'query', 'gandai.models', 'Search', 're', 'pandas', 'pd', 'DataFrame', 'dealcloud_company_query', 'dealcloud_engagements', 'migrate_engagements')
+   names      ('gandai', 'query', 'gandai.models', 'Search', 're', 'pandas', 'pd', 'DataFrame', 'dealcloud_company_query', 'dealcloud_engagements', 'migrate_engagements', 'main', '__name__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c020801080318160815
+   lnotab
+      0x00ff02010c010c020801080402ff04020cfe08190815062206040c0118
+      ff
```

### Comparing `gandai-1.1.6/gandai/migrations/db_seed.py` & `gandai-1.1.7/gandai/migrations/db_seed.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,15 @@
             search_uid=search.uid,
             domain=company.domain,
             actor_key="7138248581",
             type="create",
         )
     )
 
-# def seed_searches():
-
 
 def main():
-    # seed_actors()
-    # seed_hello_world()
-    migrate_engagements()
+    seed_actors()
+    seed_hello_world()
     
 
 if __name__ == "__main__":
     main()
```

### Comparing `gandai-1.1.6/gandai/migrations/dealcloud.py` & `gandai-1.1.7/gandai/migrations/dealcloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from gandai import query
 from gandai.models import Search
 
 import re
 import pandas as pd
 
 
-def dealcloud_company_query(fp="data/company.xlsx") -> pd.DataFrame:
+def dealcloud_company_query(
+    fp="/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx",
+) -> pd.DataFrame:
     print("dealcloud_company_query")
+
     def _get_domain(url) -> str:
         url = url.replace("http://", "").replace("https://", "").replace("www.", "")
         return url.split("/")[0]
 
     df = pd.read_excel(fp)  # hmm why so slow, maybe just select specific columns?
     df.columns = [col.replace(" ", "_").replace(".", "").lower() for col in df.columns]
     assert "dealcloud_id" in df.columns
     df["domain"] = df["website"].dropna().apply(_get_domain)
     df["days_since_contact"] = (
         df["days_since_contact"].dropna().apply(lambda x: int(re.findall(r"\d+", x)[0]))
     )
-    df = df.rename(columns={"company_name": "name"})
+    df = df.rename(
+        columns={"company_name": "name", "business_description": "description"}
+    )
     # df = (
     #     df[["dealcloud_id","name", "domain", "days_since_contact"]]
     #     .drop_duplicates(subset=["domain"])
     #     .reset_index(drop=True)
     # )
     return df
 
@@ -75,7 +80,15 @@
                 "country": ["USA"],
                 "employees_range": [10, 100],
             },
             sort={"field": "domain", "order": "desc"},
         )
         print(search)
         query.insert_search(search)
+
+
+def main():
+    migrate_engagements()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `gandai-1.1.6/gandai/migrations/sql/schema.sql` & `gandai-1.1.7/gandai/migrations/sql/schema.sql`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     sort JSONB DEFAULT '{}'::jsonb,
     created BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW())),
     updated BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW()))
 );
 
 CREATE TABLE IF NOT EXISTS company (
     id SERIAL PRIMARY KEY,
+    uid INTEGER UNIQUE,
     domain VARCHAR(255) UNIQUE NOT NULL,
     name VARCHAR(255),
     description TEXT,
     meta JSONB DEFAULT '{}'::jsonb, 
     created BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW())),
     updated BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW()))
 
@@ -58,15 +59,15 @@
     e.domain, 
     e.data, 
     e.type AS last_event_type, 
     e.created AS last_event_dt,
     c.name as name,
     c.description as description,
     c.meta as meta,
-    (c.meta->>'employees')::int AS employees,
+    (c.meta->>'employees')::INTEGER AS employees,
     (c.meta->>'ownership_status') AS ownership_status,
     (c.meta->>'social_linkedin') AS linkedin,    
     (r.data->>'rating')::int AS rating
 FROM (
     SELECT 
         domain, 
         MAX(created) AS max_created
```

### Comparing `gandai-1.1.6/gandai/models.py` & `gandai-1.1.7/gandai/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @dataclass(order=True)
 class Company:
     domain: str  # unique
     name: Optional[str] = None
     description: Optional[str] = None
     meta: dict = field(default_factory=dict)
     id: int = field(default=None)  # primary key
+    uid: int = field(default=None)  # foreign key
 
 
 class EventType(str, Enum):
     CREATE = auto()
     ADVANCE = auto()
     VALIDATE = auto()
     SEND = auto()
```

### Comparing `gandai-1.1.6/gandai/query.py` & `gandai-1.1.7/gandai/query.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai/sources.py` & `gandai-1.1.7/gandai/sources.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.6/gandai.egg-info/SOURCES.txt` & `gandai-1.1.7/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

