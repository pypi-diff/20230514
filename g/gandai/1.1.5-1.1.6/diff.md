# Comparing `tmp/gandai-1.1.5.tar.gz` & `tmp/gandai-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.1.5.tar", last modified: Sat May 13 20:22:51 2023, max compression
+gzip compressed data, was "gandai-1.1.6.tar", last modified: Sun May 14 02:15:01 2023, max compression
```

## Comparing `gandai-1.1.5.tar` & `gandai-1.1.6.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-13 20:22:51.218492 gandai-1.1.5/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.5/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-13 20:22:51.218361 gandai-1.1.5/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-13 20:22:51.213620 gandai-1.1.5/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.5/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-13 20:22:51.217116 gandai-1.1.5/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.5/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.5/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.5/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4152 2023-04-12 13:11:27.000000 gandai-1.1.5/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.5/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.5/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5068 2023-05-12 19:30:40.000000 gandai-1.1.5/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6064 2023-05-12 19:41:17.000000 gandai-1.1.5/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    15927 2023-05-13 19:31:21.000000 gandai-1.1.5/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.5/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7849 2023-05-12 19:25:42.000000 gandai-1.1.5/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1699 2023-05-13 19:58:43.000000 gandai-1.1.5/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.5/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     3286 2023-05-12 19:30:37.000000 gandai-1.1.5/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-13 20:22:51.217662 gandai-1.1.5/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.5/gandai/migrations/__init__.py
--rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.5/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1565 2023-05-13 19:29:54.000000 gandai-1.1.5/gandai/migrations/db_seed.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-13 20:22:51.217915 gandai-1.1.5/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)     2815 2023-05-13 19:15:16.000000 gandai-1.1.5/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2592 2023-05-12 19:41:16.000000 gandai-1.1.5/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)     8401 2023-05-13 19:31:13.000000 gandai-1.1.5/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     5418 2023-05-12 19:25:41.000000 gandai-1.1.5/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-13 20:22:51.214314 gandai-1.1.5/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-13 20:22:51.000000 gandai-1.1.5/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)      853 2023-05-13 20:22:51.000000 gandai-1.1.5/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-13 20:22:51.000000 gandai-1.1.5/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-13 20:22:51.000000 gandai-1.1.5/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-13 20:22:42.000000 gandai-1.1.5/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-13 20:22:51.218530 gandai-1.1.5/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.5/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.195051 gandai-1.1.6/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.6/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-14 02:15:01.194928 gandai-1.1.6/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.189261 gandai-1.1.6/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.6/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.192817 gandai-1.1.6/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.6/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.6/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.6/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4064 2023-05-14 00:47:34.000000 gandai-1.1.6/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.6/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.6/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5068 2023-05-12 19:30:40.000000 gandai-1.1.6/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6064 2023-05-12 19:41:17.000000 gandai-1.1.6/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    16436 2023-05-14 01:24:41.000000 gandai-1.1.6/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.6/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7849 2023-05-12 19:25:42.000000 gandai-1.1.6/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1699 2023-05-13 19:58:43.000000 gandai-1.1.6/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1583 2023-05-14 00:47:07.000000 gandai-1.1.6/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.6/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     3286 2023-05-12 19:30:37.000000 gandai-1.1.6/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.193842 gandai-1.1.6/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.6/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.194320 gandai-1.1.6/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.1.6/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6097 2023-05-13 21:29:04.000000 gandai-1.1.6/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.6/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1680 2023-05-13 21:28:48.000000 gandai-1.1.6/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3043 2023-05-14 01:40:03.000000 gandai-1.1.6/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.194663 gandai-1.1.6/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)     2815 2023-05-13 19:15:16.000000 gandai-1.1.6/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2592 2023-05-12 19:41:16.000000 gandai-1.1.6/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)     8697 2023-05-14 01:24:23.000000 gandai-1.1.6/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     5442 2023-05-14 02:14:15.000000 gandai-1.1.6/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 02:15:01.189798 gandai-1.1.6/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-14 02:15:01.000000 gandai-1.1.6/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1015 2023-05-14 02:15:01.000000 gandai-1.1.6/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-14 02:15:01.000000 gandai-1.1.6/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-14 02:15:01.000000 gandai-1.1.6/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-14 02:14:55.000000 gandai-1.1.6/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-14 02:15:01.195082 gandai-1.1.6/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.6/setup.py
```

### Comparing `gandai-1.1.5/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files 26% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0xfead3664 (Wed Apr 12 13:11:26 2023 UTC)
-files sz: 1578
+moddate:  0x8b2f6064 (Sun May 14 00:47:07 2023 UTC)
+files sz: 1583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       026c036d045a040100640064036c056d065a066d075a076d085a08010064
-      0064046c096d0a5a0a0100640064016c025a02640064056c0b6d0c5a0c01
-      000200650ca6000000ab0000000000000000000100020047006406840064
-      07a6020000ab0200000000000000005a0d64015300
+      0064046c096d0a5a0a0100640064016c025a0202004700640584006406a6
+      020000ab0200000000000000005a0b64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (datetime)
                  8 STORE_NAME               0 (datetime)
    
@@ -55,44 +54,30 @@
                 68 POP_TOP
    
      8          70 LOAD_CONST               0 (0)
                 72 LOAD_CONST               1 (None)
                 74 IMPORT_NAME              2 (os)
                 76 STORE_NAME               2 (os)
    
-     9          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               5 (('load_dotenv',))
-                82 IMPORT_NAME             11 (dotenv)
-                84 IMPORT_FROM             12 (load_dotenv)
-                86 STORE_NAME              12 (load_dotenv)
-                88 POP_TOP
-   
-    10          90 PUSH_NULL
-                92 LOAD_NAME               12 (load_dotenv)
-                94 PRECALL                  0
-                98 CALL                     0
-               108 POP_TOP
-   
-    12         110 PUSH_NULL
-               112 LOAD_BUILD_CLASS
-               114 LOAD_CONST               6 (<code object Cloudstore, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 12>)
-               116 MAKE_FUNCTION            0
-               118 LOAD_CONST               7 ('Cloudstore')
-               120 PRECALL                  2
-               124 CALL                     2
-               134 STORE_NAME              13 (Cloudstore)
-               136 LOAD_CONST               1 (None)
-               138 RETURN_VALUE
+    12          78 PUSH_NULL
+                80 LOAD_BUILD_CLASS
+                82 LOAD_CONST               5 (<code object Cloudstore, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py", line 12>)
+                84 MAKE_FUNCTION            0
+                86 LOAD_CONST               6 ('Cloudstore')
+                88 PRECALL                  2
+                92 CALL                     2
+               102 STORE_NAME              11 (Cloudstore)
+               104 LOAD_CONST               1 (None)
+               106 RETURN_VALUE
    consts
       0
       None
       ('ThreadPoolExecutor',)
       ('Any', 'Dict', 'List')
       ('storage',)
-      ('load_dotenv',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640d6403650465051900000000
@@ -178,23 +163,23 @@
                   00000000000000000000000000000000007c006a020000000000000000a6
                   010000ab0100000000000000007c005f07000000000000000064005300
                 13           0 RESUME                   0
                
                 14           2 LOAD_GLOBAL              1 (NULL + os)
                             14 LOAD_ATTR                1 (getenv)
                             24 LOAD_CONST               1 ('GCP_PROJECT')
-                            26 LOAD_CONST               2 ('gandai-beta')
+                            26 LOAD_CONST               2 ('gandai-prod')
                             28 PRECALL                  2
                             32 CALL                     2
                             42 STORE_FAST               1 (GCP_PROJECT)
                
                 15          44 LOAD_GLOBAL              1 (NULL + os)
                             56 LOAD_ATTR                1 (getenv)
                             66 LOAD_CONST               3 ('GCP_STAGE')
-                            68 LOAD_CONST               4 ('dev')
+                            68 LOAD_CONST               4 ('prod')
                             70 PRECALL                  2
                             74 CALL                     2
                             84 STORE_FAST               2 (GCP_STAGE)
                
                 16          86 LOAD_FAST                1 (GCP_PROJECT)
                             88 FORMAT_VALUE             0
                             90 LOAD_CONST               5 ('-')
@@ -223,17 +208,17 @@
                            222 LOAD_FAST                0 (self)
                            224 STORE_ATTR               7 (bucket)
                            234 LOAD_CONST               0 (None)
                            236 RETURN_VALUE
                consts
                   None
                   'GCP_PROJECT'
-                  'gandai-beta'
+                  'gandai-prod'
                   'GCP_STAGE'
-                  'dev'
+                  'prod'
                   '-'
                   ('project',)
                names      ('os', 'getenv', 'BUCKET_NAME', 'storage', 'Client', 'client', 'get_bucket', 'bucket')
                varnames   ('self', 'GCP_PROJECT', 'GCP_STAGE')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
@@ -571,15 +556,15 @@
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
          name       'Cloudstore'
          firstlineno 12
          lnotab 0x0a0106071a071004100410040605
       'Cloudstore'
-   names      ('datetime', 'json', 'os', 'concurrent.futures', 'ThreadPoolExecutor', 'typing', 'Any', 'Dict', 'List', 'google.cloud', 'storage', 'dotenv', 'load_dotenv', 'Cloudstore')
+   names      ('datetime', 'json', 'os', 'concurrent.futures', 'ThreadPoolExecutor', 'typing', 'Any', 'Dict', 'List', 'google.cloud', 'storage', 'Cloudstore')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/datastore.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010801080108010c0214010c0108010c011402
+   lnotab 0x00ff02010801080108010c0214010c010804
```

### Comparing `gandai-1.1.5/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,31 +1,31 @@
 magic:    0xa70d0d0a
-moddate:  0x81e55f64 (Sat May 13 19:31:13 2023 UTC)
-files sz: 8401
+moddate:  0x47386064 (Sun May 14 01:24:23 2023 UTC)
+files sz: 8697
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064026c036d045a0401
       00640064036c056d065a060100640064046c076d085a086d095a096d0a5a
       0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064016c0e5a0e640064056c0f6d
       105a100100640064066c116d125a12010002006512a6000000ab00000000
       00000000000100640064076c136d145a14010002006514a6000000ab0000
       000000000000005a15640865096602640984045a16640a6508640b650866
       04640c84045a17640d650b640b650b6604640e84045a18640f650c640b65
       0c6604641084045a196411650d640b650d6604641284045a1a641384005a
-      1b64206414651c6415651d6604641684055a1e6414651c640b65026a1f00
+      1b64216414651c6415651d6604641684055a1e6414651c640b65026a1f00
       000000000000006604641784045a206414651c640b65026a1f0000000000
       0000006604641884045a21640b65026a1f00000000000000006602641984
-      045a226414651c640b65026a1f00000000000000006604641a84045a2364
-      14651c640b650c6604641b84045a24641c651d640b65096604641d84045a
-      2564086509640b64016604641e84045a26640f650c640b64016604641f84
-      045a2764015300
+      045a22640b65026a1f00000000000000006602641a84045a236414651c64
+      0b65026a1f00000000000000006604641b84045a246414651c640b650c66
+      04641c84045a25641d651d640b65096604641e84045a2664086509640b64
+      016604641f84045a27640f650c640b64016604642084045a2864015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (json)
                  8 STORE_NAME               0 (json)
    
@@ -146,15 +146,15 @@
                230 MAKE_FUNCTION            4 (annotations)
                232 STORE_NAME              26 (insert_checkpoint)
    
    114         234 LOAD_CONST              19 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 114>)
                236 MAKE_FUNCTION            0
                238 STORE_NAME              27 (search)
    
-   121         240 LOAD_CONST              32 ((None,))
+   121         240 LOAD_CONST              33 ((None,))
                242 LOAD_CONST              20 ('search_uid')
                244 LOAD_NAME               28 (int)
                246 LOAD_CONST              21 ('last_event_type')
                248 LOAD_NAME               29 (str)
                250 BUILD_TUPLE              4
                252 LOAD_CONST              22 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 121>)
                254 MAKE_FUNCTION            5 (defaults, annotations)
@@ -176,69 +176,77 @@
                290 LOAD_NAME                2 (pd)
                292 LOAD_ATTR               31 (DataFrame)
                302 BUILD_TUPLE              4
                304 LOAD_CONST              24 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 169>)
                306 MAKE_FUNCTION            4 (annotations)
                308 STORE_NAME              33 (event)
    
-   181         310 LOAD_CONST              11 ('return')
+   180         310 LOAD_CONST              11 ('return')
                312 LOAD_NAME                2 (pd)
                314 LOAD_ATTR               31 (DataFrame)
                324 BUILD_TUPLE              2
-               326 LOAD_CONST              25 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 181>)
+               326 LOAD_CONST              25 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 180>)
                328 MAKE_FUNCTION            4 (annotations)
-               330 STORE_NAME              34 (checkpoint)
+               330 STORE_NAME              34 (company)
    
-   192         332 LOAD_CONST              20 ('search_uid')
-               334 LOAD_NAME               28 (int)
-               336 LOAD_CONST              11 ('return')
-               338 LOAD_NAME                2 (pd)
-               340 LOAD_ATTR               31 (DataFrame)
-               350 BUILD_TUPLE              4
-               352 LOAD_CONST              26 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 192>)
-               354 MAKE_FUNCTION            4 (annotations)
-               356 STORE_NAME              35 (comment_by_domain)
-   
-   213         358 LOAD_CONST              20 ('search_uid')
-               360 LOAD_NAME               28 (int)
-               362 LOAD_CONST              11 ('return')
-               364 LOAD_NAME               12 (Search)
-               366 BUILD_TUPLE              4
-               368 LOAD_CONST              27 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 213>)
-               370 MAKE_FUNCTION            4 (annotations)
-               372 STORE_NAME              36 (find_search_by_uid)
-   
-   229         374 LOAD_CONST              28 ('domain')
-               376 LOAD_NAME               29 (str)
-               378 LOAD_CONST              11 ('return')
-               380 LOAD_NAME                9 (Company)
-               382 BUILD_TUPLE              4
-               384 LOAD_CONST              29 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 229>)
-               386 MAKE_FUNCTION            4 (annotations)
-               388 STORE_NAME              37 (find_company_by_domain)
-   
-   248         390 LOAD_CONST               8 ('company')
-               392 LOAD_NAME                9 (Company)
-               394 LOAD_CONST              11 ('return')
-               396 LOAD_CONST               1 (None)
-               398 BUILD_TUPLE              4
-               400 LOAD_CONST              30 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 248>)
-               402 MAKE_FUNCTION            4 (annotations)
-               404 STORE_NAME              38 (update_company)
-   
-   272         406 LOAD_CONST              15 ('search')
-               408 LOAD_NAME               12 (Search)
-               410 LOAD_CONST              11 ('return')
-               412 LOAD_CONST               1 (None)
-               414 BUILD_TUPLE              4
-               416 LOAD_CONST              31 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 272>)
-               418 MAKE_FUNCTION            4 (annotations)
-               420 STORE_NAME              39 (update_search)
-               422 LOAD_CONST               1 (None)
-               424 RETURN_VALUE
+   190         332 LOAD_CONST              11 ('return')
+               334 LOAD_NAME                2 (pd)
+               336 LOAD_ATTR               31 (DataFrame)
+               346 BUILD_TUPLE              2
+               348 LOAD_CONST              26 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 190>)
+               350 MAKE_FUNCTION            4 (annotations)
+               352 STORE_NAME              35 (checkpoint)
+   
+   201         354 LOAD_CONST              20 ('search_uid')
+               356 LOAD_NAME               28 (int)
+               358 LOAD_CONST              11 ('return')
+               360 LOAD_NAME                2 (pd)
+               362 LOAD_ATTR               31 (DataFrame)
+               372 BUILD_TUPLE              4
+               374 LOAD_CONST              27 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 201>)
+               376 MAKE_FUNCTION            4 (annotations)
+               378 STORE_NAME              36 (comment_by_domain)
+   
+   222         380 LOAD_CONST              20 ('search_uid')
+               382 LOAD_NAME               28 (int)
+               384 LOAD_CONST              11 ('return')
+               386 LOAD_NAME               12 (Search)
+               388 BUILD_TUPLE              4
+               390 LOAD_CONST              28 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 222>)
+               392 MAKE_FUNCTION            4 (annotations)
+               394 STORE_NAME              37 (find_search_by_uid)
+   
+   238         396 LOAD_CONST              29 ('domain')
+               398 LOAD_NAME               29 (str)
+               400 LOAD_CONST              11 ('return')
+               402 LOAD_NAME                9 (Company)
+               404 BUILD_TUPLE              4
+               406 LOAD_CONST              30 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 238>)
+               408 MAKE_FUNCTION            4 (annotations)
+               410 STORE_NAME              38 (find_company_by_domain)
+   
+   257         412 LOAD_CONST               8 ('company')
+               414 LOAD_NAME                9 (Company)
+               416 LOAD_CONST              11 ('return')
+               418 LOAD_CONST               1 (None)
+               420 BUILD_TUPLE              4
+               422 LOAD_CONST              31 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 257>)
+               424 MAKE_FUNCTION            4 (annotations)
+               426 STORE_NAME              39 (update_company)
+   
+   281         428 LOAD_CONST              15 ('search')
+               430 LOAD_NAME               12 (Search)
+               432 LOAD_CONST              11 ('return')
+               434 LOAD_CONST               1 (None)
+               436 BUILD_TUPLE              4
+               438 LOAD_CONST              32 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 281>)
+               440 MAKE_FUNCTION            4 (annotations)
+               442 STORE_NAME              40 (update_search)
+               444 LOAD_CONST               1 (None)
+               446 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('from_dict',)
       ('Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint')
       ('Connector',)
@@ -1285,53 +1293,53 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d03640064006400a6020000ab020000000000
             00000001006e0b230031007304770278035900770101005900010001007c
             035300
-         181           0 RESUME                   0
+         180           0 RESUME                   0
          
-         182           2 LOAD_GLOBAL              0 (db)
+         181           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         183          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n            ')
+         182          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
                       56 STORE_FAST               1 (statement)
          
-         187          58 LOAD_FAST                0 (conn)
+         186          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         188         136 LOAD_GLOBAL             11 (NULL + pd)
+         187         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         182         252 LOAD_CONST               0 (None)
+         181         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -1342,15 +1350,107 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         189     >>  298 LOAD_FAST                3 (df)
+         188     >>  298 LOAD_FAST                3 (df)
+                     300 RETURN_VALUE
+         ExceptionTable:
+           52 to 250 -> 276 [1] lasti
+           276 to 282 -> 284 [3] lasti
+           290 to 290 -> 284 [3] lasti
+         consts
+            None
+            '\n                SELECT *\n                FROM company\n            '
+            ('columns',)
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
+         varnames   ('conn', 'statement', 'result', 'df')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'company'
+         firstlineno 180
+         lnotab 0x0201340104044e0174fa2e07
+      code
+         argcount  : 0
+         nlocals   : 4
+         stacksize : 6
+         flags     : 3
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            00000000000000a6000000ab00000000000000000035007d0064017d017c
+            00a002000000000000000000000000000000000000000074070000000000
+            00000000006a0400000000000000007c01a6010000ab0100000000000000
+            00a6010000ab0100000000000000007d02740b000000000000000000006a
+            0600000000000000007c02a0070000000000000000000000000000000000
+            000000a6000000ab0000000000000000007c02a008000000000000000000
+            0000000000000000000000a6000000ab000000000000000000ac02a60200
+            00ab0200000000000000007d03640064006400a6020000ab020000000000
+            00000001006e0b230031007304770278035900770101005900010001007c
+            035300
+         190           0 RESUME                   0
+         
+         191           2 LOAD_GLOBAL              0 (db)
+                      14 LOAD_METHOD              1 (connect)
+                      36 PRECALL                  0
+                      40 CALL                     0
+                      50 BEFORE_WITH
+                      52 STORE_FAST               0 (conn)
+         
+         192          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n            ')
+                      56 STORE_FAST               1 (statement)
+         
+         196          58 LOAD_FAST                0 (conn)
+                      60 LOAD_METHOD              2 (execute)
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                1 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 PRECALL                  1
+                     124 CALL                     1
+                     134 STORE_FAST               2 (result)
+         
+         197         136 LOAD_GLOBAL             11 (NULL + pd)
+                     148 LOAD_ATTR                6 (DataFrame)
+                     158 LOAD_FAST                2 (result)
+                     160 LOAD_METHOD              7 (fetchall)
+                     182 PRECALL                  0
+                     186 CALL                     0
+                     196 LOAD_FAST                2 (result)
+                     198 LOAD_METHOD              8 (keys)
+                     220 PRECALL                  0
+                     224 CALL                     0
+                     234 KW_NAMES                 2
+                     236 PRECALL                  2
+                     240 CALL                     2
+                     250 STORE_FAST               3 (df)
+         
+         191         252 LOAD_CONST               0 (None)
+                     254 LOAD_CONST               0 (None)
+                     256 LOAD_CONST               0 (None)
+                     258 PRECALL                  2
+                     262 CALL                     2
+                     272 POP_TOP
+                     274 JUMP_FORWARD            11 (to 298)
+                 >>  276 PUSH_EXC_INFO
+                     278 WITH_EXCEPT_START
+                     280 POP_JUMP_FORWARD_IF_TRUE     4 (to 290)
+                     282 RERAISE                  2
+                 >>  284 COPY                     3
+                     286 POP_EXCEPT
+                     288 RERAISE                  1
+                 >>  290 POP_TOP
+                     292 POP_EXCEPT
+                     294 POP_TOP
+                     296 POP_TOP
+         
+         198     >>  298 LOAD_FAST                3 (df)
                      300 RETURN_VALUE
          ExceptionTable:
            52 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -1358,15 +1458,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'checkpoint'
-         firstlineno 181
+         firstlineno 190
          lnotab 0x0201340104044e0174fa2e07
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -1381,59 +1481,59 @@
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c04a009000000000000000000000000000000000000000064
             04a6010000ab010000000000000000a00a00000000000000000000000000
             000000000000006405640684006901a6010000ab010000000000000000a0
             0b0000000000000000000000000000000000000000a6000000ab00000000
             00000000005300
-         192           0 RESUME                   0
+         201           0 RESUME                   0
          
-         193           2 LOAD_GLOBAL              0 (db)
+         202           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         194          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
+         203          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
                       56 STORE_FAST               2 (statement)
          
-         201          58 LOAD_FAST                1 (conn)
+         210          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         202          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         211          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         203         120 LOAD_CONST               2 ('search_uid')
+         212         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         201         126 PRECALL                  2
+         210         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         205         142 LOAD_GLOBAL             11 (NULL + pd)
+         214         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         193         258 LOAD_CONST               0 (None)
+         202         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -1444,22 +1544,22 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         207     >>  304 LOAD_FAST                4 (df)
+         216     >>  304 LOAD_FAST                4 (df)
                      306 LOAD_METHOD              9 (groupby)
                      328 LOAD_CONST               4 ('domain')
                      330 PRECALL                  1
                      334 CALL                     1
                      344 LOAD_METHOD             10 (agg)
                      366 LOAD_CONST               5 ('comment')
-                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 207>)
+                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 216>)
                      370 MAKE_FUNCTION            0
                      372 BUILD_MAP                1
                      374 PRECALL                  1
                      378 CALL                     1
                      388 LOAD_METHOD             11 (reset_index)
                      410 PRECALL                  0
                      414 CALL                     0
@@ -1479,37 +1579,37 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               207           0 RESUME                   0
+               216           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('list',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 207
+               firstlineno 216
                lnotab 0x
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'comment_by_domain'
-         firstlineno 192
+         firstlineno 201
          lnotab 0x0201340104071801260106fe100474f42e0e
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
@@ -1522,41 +1622,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         213           0 RESUME                   0
+         222           0 RESUME                   0
          
-         214           2 LOAD_GLOBAL              0 (db)
+         223           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         215          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
+         224          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         220          58 LOAD_FAST                1 (conn)
+         229          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         214         142 LOAD_CONST               0 (None)
+         223         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -1567,24 +1667,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         222     >>  188 LOAD_FAST                3 (result)
+         231     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         223         210 LOAD_CONST               0 (None)
+         232         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         225     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         234     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -1592,15 +1692,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         226         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         235         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Search)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -1613,15 +1713,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_uid'
-         firstlineno 213
+         firstlineno 222
          lnotab 0x02013401040554fa2e08160104028201
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -1635,41 +1735,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         229           0 RESUME                   0
+         238           0 RESUME                   0
          
-         230           2 LOAD_GLOBAL              0 (db)
+         239           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         231          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         240          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         236          58 LOAD_FAST                1 (conn)
+         245          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         230         142 LOAD_CONST               0 (None)
+         239         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -1680,24 +1780,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         238     >>  188 LOAD_FAST                3 (result)
+         247     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         239         210 LOAD_CONST               0 (None)
+         248         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         241     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         250     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -1705,15 +1805,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         242         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         251         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -1726,15 +1826,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 229
+         firstlineno 238
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 10
          flags     : 3
          code
@@ -1748,76 +1848,76 @@
             020000ab02000000000000000001007c01a0020000000000000000000000
             0000000000000000007407000000000000000000006a0400000000000000
             006403a6010000ab010000000000000000a6010000ab0100000000000000
             0001007c01a00b0000000000000000000000000000000000000000a60000
             00ab0000000000000000000100640064006400a6020000ab020000000000
             000000010064005300230031007304770278035900770101005900010001
             0064005300
-         248           0 RESUME                   0
+         257           0 RESUME                   0
          
-         249           2 LOAD_GLOBAL              0 (db)
+         258           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         250          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
+         259          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         259          58 LOAD_FAST                1 (conn)
+         268          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         260          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         269          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         262         120 LOAD_FAST                0 (company)
+         271         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (name)
          
-         263         132 LOAD_FAST                0 (company)
+         272         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (description)
          
-         264         144 LOAD_FAST                0 (company)
+         273         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (domain)
          
-         265         156 LOAD_GLOBAL             17 (NULL + json)
+         274         156 LOAD_GLOBAL             17 (NULL + json)
                      168 LOAD_ATTR                9 (dumps)
                      178 LOAD_FAST                0 (company)
                      180 LOAD_ATTR               10 (meta)
                      190 PRECALL                  1
                      194 CALL                     1
          
-         261         204 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
+         270         204 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
                      206 BUILD_CONST_KEY_MAP      4
          
-         259         208 PRECALL                  2
+         268         208 PRECALL                  2
                      212 CALL                     2
                      222 POP_TOP
          
-         268         224 LOAD_FAST                1 (conn)
+         277         224 LOAD_FAST                1 (conn)
                      226 LOAD_METHOD              2 (execute)
                      248 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      260 LOAD_ATTR                4 (text)
                      270 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW target')
                      272 PRECALL                  1
                      276 CALL                     1
                      286 PRECALL                  1
                      290 CALL                     1
                      300 POP_TOP
          
-         269         302 LOAD_FAST                1 (conn)
+         278         302 LOAD_FAST                1 (conn)
                      304 LOAD_METHOD             11 (commit)
                      326 PRECALL                  0
                      330 CALL                     0
                      340 POP_TOP
          
-         249         342 LOAD_CONST               0 (None)
+         258         342 LOAD_CONST               0 (None)
                      344 LOAD_CONST               0 (None)
                      346 LOAD_CONST               0 (None)
                      348 PRECALL                  2
                      352 CALL                     2
                      362 POP_TOP
                      364 LOAD_CONST               0 (None)
                      366 RETURN_VALUE
@@ -1845,15 +1945,15 @@
             'REFRESH MATERIALIZED VIEW target'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 248
+         firstlineno 257
          lnotab 0x020134010409180126020c010c010c0130fc04fe10094e0128ec
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 9
          flags     : 3
          code
@@ -1866,72 +1966,72 @@
             000000000000007c006a080000000000000000a6010000ab010000000000
             000000740b000000000000000000006a0600000000000000007c006a0900
             00000000000000a6010000ab0100000000000000007c006a0a0000000000
             00000064029c04a6020000ab02000000000000000001007c01a00b000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             000100640064006400a6020000ab02000000000000000001006400530023
             00310073047702780359007701010059000100010064005300
-         272           0 RESUME                   0
+         281           0 RESUME                   0
          
-         273           2 LOAD_GLOBAL              0 (db)
+         282           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         274          54 LOAD_FAST                1 (conn)
+         283          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         275          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         284          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         276         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
+         285         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
          
-         275         102 PRECALL                  1
+         284         102 PRECALL                  1
                      106 CALL                     1
          
-         286         116 LOAD_GLOBAL             11 (NULL + json)
+         295         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (sort)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         287         164 LOAD_GLOBAL             11 (NULL + json)
+         296         164 LOAD_GLOBAL             11 (NULL + json)
                      176 LOAD_ATTR                6 (dumps)
                      186 LOAD_FAST                0 (search)
                      188 LOAD_ATTR                8 (inclusion)
                      198 PRECALL                  1
                      202 CALL                     1
          
-         288         212 LOAD_GLOBAL             11 (NULL + json)
+         297         212 LOAD_GLOBAL             11 (NULL + json)
                      224 LOAD_ATTR                6 (dumps)
                      234 LOAD_FAST                0 (search)
                      236 LOAD_ATTR                9 (exclusion)
                      246 PRECALL                  1
                      250 CALL                     1
          
-         289         260 LOAD_FAST                0 (search)
+         298         260 LOAD_FAST                0 (search)
                      262 LOAD_ATTR               10 (uid)
          
-         285         272 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
+         294         272 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
                      274 BUILD_CONST_KEY_MAP      4
          
-         274         276 PRECALL                  2
+         283         276 PRECALL                  2
                      280 CALL                     2
                      290 POP_TOP
          
-         292         292 LOAD_FAST                1 (conn)
+         301         292 LOAD_FAST                1 (conn)
                      294 LOAD_METHOD             11 (commit)
                      316 PRECALL                  0
                      320 CALL                     0
                      330 POP_TOP
          
-         273         332 LOAD_CONST               0 (None)
+         282         332 LOAD_CONST               0 (None)
                      334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 PRECALL                  2
                      342 CALL                     2
                      352 POP_TOP
                      354 LOAD_CONST               0 (None)
                      356 RETURN_VALUE
@@ -1958,20 +2058,20 @@
             ('sort', 'inclusion', 'exclusion', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 272
+         firstlineno 281
          lnotab 0x020134011801160102ff0e0b3001300130010cfc04f5101228ed
       (None,)
-   names      ('json', 'pandas', 'pd', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'sqlalchemy', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'gandai.db', 'connect_with_connector', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'search', 'int', 'str', 'target', 'DataFrame', 'target_count', 'event', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'update_company', 'update_search')
+   names      ('json', 'pandas', 'pd', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'sqlalchemy', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'gandai.db', 'connect_with_connector', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'search', 'int', 'str', 'target', 'DataFrame', 'target_count', 'event', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'update_company', 'update_search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c01200a08020c010c0114020c0214060c0e10
-      15100f10131010060712201a101a0c160b1a15101010131018
+      15100f10131010060712201a101a0b160a160b1a15101010131018
```

### Comparing `gandai-1.1.5/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.1.6/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/auth.py` & `gandai-1.1.6/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/db.py` & `gandai-1.1.6/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/main.py` & `gandai-1.1.6/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/migrations/db_seed.py` & `gandai-1.1.6/gandai/migrations/db_seed.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from gandai import query
 from gandai.models import Company, Actor, Search, Event
+from gandai.migrations.dealcloud import migrate_engagements
 
 def seed_actors():
     actors = {
         "7138248581": "Parker",
         "6508620943": "Gabe",
         "9413500954": "Skye",
         "3102835279": "Chris",
@@ -49,14 +50,18 @@
             search_uid=search.uid,
             domain=company.domain,
             actor_key="7138248581",
             type="create",
         )
     )
 
+# def seed_searches():
+
+
 def main():
-    seed_actors()
-    seed_hello_world()
+    # seed_actors()
+    # seed_hello_world()
+    migrate_engagements()
     
 
 if __name__ == "__main__":
     main()
```

### Comparing `gandai-1.1.5/gandai/migrations/sql/schema.sql` & `gandai-1.1.6/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/models.py` & `gandai-1.1.6/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.5/gandai/query.py` & `gandai-1.1.6/gandai/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,23 @@
                 FROM event
                 WHERE search_uid = :search_uid
             """
         result = conn.execute(sqlalchemy.text(statement), {"search_uid": search_uid})
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     return df
 
+def company() -> pd.DataFrame:
+    with db.connect() as conn:
+        statement = """
+                SELECT *
+                FROM company
+            """
+        result = conn.execute(sqlalchemy.text(statement))
+        df = pd.DataFrame(result.fetchall(), columns=result.keys())
+    return df
 
 def checkpoint() -> pd.DataFrame:
     with db.connect() as conn:
         statement = """
                 SELECT *
                 FROM checkpoint
             """
```

### Comparing `gandai-1.1.5/gandai/sources.py` & `gandai-1.1.6/gandai/sources.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,17 +147,17 @@
             exclude = []
             for state in search.exclusion.get("state", []):
                 exclude.append({"state": state})
             return exclude
 
         return {
             "op": "any",
-            "include": search.inclusion["keywords"],
-            "exclude": search.exclusion["keywords"],
-            "employees_range": search.inclusion["employees_range"],
+            "include": search.inclusion.get("keywords", []),
+            "exclude": search.exclusion.get("keywords", []),
+            "employees_range": search.inclusion.get("employees_range", []),
             "ownership": _ownership_filter(),
             "headquarters": {
                 "include": _hq_include(),
                 "exclude": _hq_exclude(),
             },
         }
```

### Comparing `gandai-1.1.5/gandai.egg-info/SOURCES.txt` & `gandai-1.1.6/gandai.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 pyproject.toml
 setup.py
 gandai/__init__.py
 gandai/auth.py
+gandai/datastore.py
 gandai/db.py
 gandai/main.py
 gandai/models.py
 gandai/query.py
 gandai/sources.py
 gandai.egg-info/PKG-INFO
 gandai.egg-info/SOURCES.txt
@@ -22,8 +23,11 @@
 gandai/__pycache__/models.cpython-311.pyc
 gandai/__pycache__/query.cpython-311.pyc
 gandai/__pycache__/services.cpython-311.pyc
 gandai/__pycache__/sources.cpython-311.pyc
 gandai/migrations/__init__.py
 gandai/migrations/db_create.py
 gandai/migrations/db_seed.py
+gandai/migrations/dealcloud.py
+gandai/migrations/__pycache__/__init__.cpython-311.pyc
+gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
 gandai/migrations/sql/schema.sql
```

