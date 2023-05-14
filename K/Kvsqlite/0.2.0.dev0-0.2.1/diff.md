# Comparing `tmp/Kvsqlite-0.2.0.dev0.tar.gz` & `tmp/Kvsqlite-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kvsqlite-0.2.0.dev0.tar", last modified: Wed Apr 26 10:15:30 2023, max compression
+gzip compressed data, was "Kvsqlite-0.2.1.tar", last modified: Sun May 14 12:30:03 2023, max compression
```

## Comparing `Kvsqlite-0.2.0.dev0.tar` & `Kvsqlite-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.545844 Kvsqlite-0.2.0.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 10:15:30.000000 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-26 10:15:30.000000 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:15:30.000000 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 10:15:30.000000 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/benchmark/benchmark_kvsqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/kvsqlite/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/kvsqlite/sync/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:15:30.545844 Kvsqlite-0.2.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/test/test_kvsqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:30:03.443359 Kvsqlite-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:30:03.443359 Kvsqlite-0.2.1/Kvsqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 12:30:03.000000 Kvsqlite-0.2.1/Kvsqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 12:30:03.000000 Kvsqlite-0.2.1/Kvsqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:30:03.000000 Kvsqlite-0.2.1/Kvsqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 12:30:03.000000 Kvsqlite-0.2.1/Kvsqlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 12:30:03.443359 Kvsqlite-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:30:03.443359 Kvsqlite-0.2.1/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/benchmark/benchmark_kvsqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:30:03.443359 Kvsqlite-0.2.1/kvsqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/kvsqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/kvsqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/kvsqlite/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/kvsqlite/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/kvsqlite/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:30:03.443359 Kvsqlite-0.2.1/kvsqlite/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/kvsqlite/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/kvsqlite/sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 12:30:03.443359 Kvsqlite-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:30:03.443359 Kvsqlite-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-14 12:30:02.000000 Kvsqlite-0.2.1/test/test_kvsqlite.py
```

### Comparing `Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/PKG-INFO` & `Kvsqlite-0.2.1/Kvsqlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kvsqlite
-Version: 0.2.0.dev0
+Version: 0.2.1
 Summary: Easy-to-use synchronous/asynchronous key-value database backed by sqlite3.
 Home-page: https://github.com/AYMENJD/Kvsqlite
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/Kvsqlite
 Project-URL: Tracker, https://github.com/AYMENJD/Kvsqlite/issues
```

### Comparing `Kvsqlite-0.2.0.dev0/LICENSE` & `Kvsqlite-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Kvsqlite-0.2.0.dev0/PKG-INFO` & `Kvsqlite-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kvsqlite
-Version: 0.2.0.dev0
+Version: 0.2.1
 Summary: Easy-to-use synchronous/asynchronous key-value database backed by sqlite3.
 Home-page: https://github.com/AYMENJD/Kvsqlite
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/Kvsqlite
 Project-URL: Tracker, https://github.com/AYMENJD/Kvsqlite/issues
```

### Comparing `Kvsqlite-0.2.0.dev0/README.md` & `Kvsqlite-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Kvsqlite-0.2.0.dev0/benchmark/benchmark_kvsqlite.py` & `Kvsqlite-0.2.1/benchmark/benchmark_kvsqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         WARNING,
         "-> Started with memory usage:",
         ENDC,
         start_memory,
     )
     for k, v in keys:
         latncey_start = time.perf_counter()
-        await db.setex(k, v, 60)
+        await db.setex(k, 60, v)
         timeing += time.perf_counter() - latncey_start
     end_memory = psutil.Process(os.getpid()).memory_info().rss
     took = time.perf_counter() - start
     print(
         WARNING,
         "-> {} query took:{} {}".format(args.query_count, ENDC, took),
     )
```

### Comparing `Kvsqlite-0.2.0.dev0/kvsqlite/base.py` & `Kvsqlite-0.2.1/kvsqlite/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import kvsqlite
-
-
 class BaseClient:
     def get(self, key: str):
         """Get the value of ``key``
 
         Args:
             key (``str``):
                 The key to get
@@ -22,29 +19,29 @@
                 The value to set for ``key``
 
         Returns:
             :py:class:`bool`: ``True`` on success
         """
         raise NotImplementedError
 
-    def setex(self, key: str, value, ttl: int):
+    def setex(self, key: str, ttl: int, value):
         """Set the value of ``key`` with a timeout specified by ``ttl``
 
         Args:
             key (``str``):
                 The key
 
-            value (``Any``):
-                The value to set for ``key``
-
             ttl (``int``):
                 The number of seconds for ``key`` timeout (a.k.a ``key`` lifetime)
 
+            value (``Any``):
+                The value to set for ``key``
+
         .. warning::
-            Timeouted keys aren't deleted by default, you must call :func:`~kvsqlite.BaseClient.cleanex` for time to time
+            Timeouted keys aren't deleted by default, you must call :func:`cleanex` from time to time
 
         Returns:
             :py:class:`bool`: ``True`` on success
         """
         raise NotImplementedError
 
     def delete(self, key: str):
```

### Comparing `Kvsqlite-0.2.0.dev0/kvsqlite/client.py` & `Kvsqlite-0.2.1/kvsqlite/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     async def set(self, key: str, value) -> bool:
         assert isinstance(key, str), "key must be str"
 
         future = self.__invoke(request=REQUEST.SET, key=key, value=value)
         return await future
 
-    async def setex(self, key: str, value, ttl: int) -> bool:
+    async def setex(self, key: str, ttl: int, value) -> bool:
         assert isinstance(key, str), "key must be str"
         assert ttl >= 1, "ttl must be greater than 1"
 
         future = self.__invoke(request=REQUEST.SETEX, key=key, value=[value, ttl])
         return await future
 
     async def delete(self, key: str) -> bool:
```

### Comparing `Kvsqlite-0.2.0.dev0/kvsqlite/encoders.py` & `Kvsqlite-0.2.1/kvsqlite/encoders.py`

 * *Files identical despite different names*

### Comparing `Kvsqlite-0.2.0.dev0/kvsqlite/sqlite.py` & `Kvsqlite-0.2.1/kvsqlite/sqlite.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,17 +21,14 @@
     RENAME = "RENAME"
     KEYS = "KEYS"
     CLEAN_EX = "CLEAN_EX"
     FLUSH_DB = "FLUSH_DB"
     CLOSE = "CLOSE"
 
 
-TABLE_STATEMENT = 'CREATE TABLE IF NOT EXISTS "{}" (k VARCHAR(4096) PRIMARY KEY, v BLOB, expire_time INTEGER DEFAULT NULL)'
-
-
 class Sqlite:
     def __init__(
         self,
         database: str,
         table_name: str,
         autocommit: bool,
         journal_mode: str,
@@ -48,19 +45,57 @@
         self.database = database
         self.table_name = table_name
         self.autocommit = autocommit
         self.journal_mode = journal_mode
         self.synchronous = synchronous
         self.__encoder = encoder
         self.__workers = ThreadPoolExecutor(workers, "kvsqlite")
-        self.__connection: sqlite3.Connection = self.__connect()
         self.__lock = Lock()
 
         self.is_running = True
 
+        self.__table_statement = 'CREATE TABLE IF NOT EXISTS "{}" (k VARCHAR(4096) PRIMARY KEY, v BLOB, expire_time INTEGER DEFAULT NULL)'.format(
+            self.table_name
+        )
+        self.__get_statement = 'SELECT v FROM "{}" WHERE k = ? AND (expire_time IS NULL OR expire_time > ?) LIMIT 1'.format(
+            self.table_name
+        )
+        self.__set_statement = (
+            'REPLACE INTO "{}" (k, v, expire_time) VALUES(?,?,NULL)'.format(
+                self.table_name
+            )
+        )
+        self.__setex_statement = (
+            'REPLACE INTO "{}" (k, v, expire_time) VALUES(?,?,?)'.format(
+                self.table_name
+            )
+        )
+        self.__delete_statement = 'DELETE FROM "{}" WHERE k = ?'.format(self.table_name)
+        self.__exists_statement = 'SELECT k FROM "{}" WHERE k = ? LIMIT 1'.format(
+            self.table_name
+        )
+        self.__ttl_statement = 'SELECT expire_time FROM "{}" WHERE k = ? AND expire_time > ? LIMIT 1'.format(
+            self.table_name
+        )
+        self.__expire_statement = 'UPDATE "{}" SET expire_time = ? WHERE k = ?'.format(
+            self.table_name
+        )
+        self.__rename_statement = 'UPDATE OR IGNORE "{}" SET k = ? WHERE k = ?'.format(
+            self.table_name
+        )
+        self.__keys_statement = (
+            'SELECT k FROM "{}" WHERE k LIKE ? ORDER BY rowid'.format(self.table_name)
+        )
+        self.__cleanex_statement = 'DELETE FROM "{}" WHERE expire_time IS NOT NULL AND expire_time <= ?'.format(
+            self.table_name
+        )
+        self.__flush_db_statement = 'DROP TABLE "{}"'.format(self.table_name)
+
+        self.__connection: sqlite3.Connection = self.__connect()
+
     def request(self, request, key: str = None, value=None):
         return self.__workers.submit(self.procces_request, request, key, value)
 
     def procces_request(self, request, key: str = None, value=None):
         if not self.is_running:
             raise RuntimeError("Database is closed")
 
@@ -126,66 +161,60 @@
             raise e
 
         return connection
 
     def __get(self, key: str):
         try:
             query = self.__connection.execute(
-                'SELECT v FROM "{}" WHERE k = ? AND (expire_time IS NULL OR expire_time > ?)'.format(
-                    self.table_name
-                ),
+                self.__get_statement,
                 (key, time()),
             ).fetchone()
             if query:
                 return self.__encoder.decode(query[0])
             else:
                 return None
         except Exception as e:
             logger.exception("GET command exception")
             raise e
 
     def __set(self, key: str, value):
         with self.__lock:
             try:
                 query = self.__connection.execute(
-                    'REPLACE INTO "{}" (k, v, expire_time) VALUES(?,?,NULL)'.format(
-                        self.table_name
-                    ),
+                    self.__set_statement,
                     (key, self.__encoder.encode(value)),
                 )
                 if query.rowcount > 0:
                     return True
                 else:
                     return False
             except Exception as e:
                 logger.exception("SET command exception")
                 raise e
 
     def __setex(self, key: str, value):
         with self.__lock:
             try:
                 query = self.__connection.execute(
-                    'REPLACE INTO "{}" (k, v, expire_time) VALUES(?,?,?)'.format(
-                        self.table_name
-                    ),
+                    self.__setex_statement,
                     (key, self.__encoder.encode(value[0]), time() + value[1]),
                 )
                 if query.rowcount > 0:
                     return True
                 else:
                     return False
             except Exception as e:
                 logger.exception("SETEX command exception")
                 raise e
 
     def __delete(self, key: str):
         with self.__lock:
             try:
                 query = self.__connection.execute(
-                    'DELETE FROM "{}" WHERE k = ?'.format(self.table_name),
+                    self.__delete_statement,
                     (key,),
                 )
                 if query.rowcount > 0:
                     return True
                 else:
                     return False
             except Exception as e:
@@ -200,32 +229,30 @@
             except Exception as e:
                 logger.exception("COMMIT command exception")
                 raise e
 
     def __exists(self, key: str):
         try:
             query = self.__connection.execute(
-                'SELECT k FROM "{}" WHERE k = ?'.format(self.table_name),
+                self.__exists_statement,
                 (key,),
             ).fetchone()
 
             if query:
                 return True
             else:
                 return False
         except Exception as e:
             logger.exception("EXISTS command exception")
             raise e
 
     def __ttl(self, key: str):
         try:
             query = self.__connection.execute(
-                'SELECT expire_time FROM "{}" WHERE k = ? AND expire_time > ?'.format(
-                    self.table_name
-                ),
+                self.__ttl_statement,
                 (key, time()),
             ).fetchone()
 
             if query:
                 return query[0] - time()
             else:
                 return 0
@@ -233,79 +260,73 @@
             logger.exception("TTL command exception")
             raise e
 
     def __expire(self, key: str, ttl: int):
         with self.__lock:
             try:
                 query = self.__connection.execute(
-                    'UPDATE "{}" SET expire_time = ? WHERE k = ?'.format(
-                        self.table_name
-                    ),
+                    self.__expire_statement,
                     (time() + ttl, key),
                 )
 
                 if query.rowcount > 0:
                     return True
                 else:
                     return False
             except Exception as e:
                 logger.exception("EXPIRE command exception")
                 raise e
 
     def __rename(self, key: str, new_key: str):
         try:
             query = self.__connection.execute(
-                'UPDATE OR IGNORE "{}" SET k = ? WHERE k = ?'.format(self.table_name),
+                self.__rename_statement,
                 (new_key, key),
             )
 
             if query.rowcount > 0:
                 return True
             else:
                 return False
         except Exception as e:
             logger.exception("RENAME command exception")
             raise e
 
     def __keys(self, like: str):
         try:
             query = self.__connection.execute(
-                'SELECT k FROM "{}" WHERE k LIKE ? ORDER BY rowid'.format(
-                    self.table_name
-                ),
+                self.__keys_statement,
                 (like,),
             ).fetchall()
             if query:
                 return query
             else:
                 return None
         except Exception as e:
             logger.exception("KEYS command exception")
             raise e
 
     def __clean_ex(self):
         with self.__lock:
             try:
                 query = self.__connection.execute(
-                    'DELETE FROM "{}" WHERE expire_time IS NOT NULL AND expire_time <= ?'.format(
-                        self.table_name
-                    ),
+                    self.__cleanex_statement,
                     (time(),),
                 )
 
                 return query.rowcount
             except Exception as e:
                 logger.exception("CLEAN_EX command exception")
                 raise e
 
     def __flush_db(self):
         with self.__lock:
             try:
-                self.__connection.execute('DROP TABLE "{}"'.format(self.table_name))
-                self.__connection.execute(TABLE_STATEMENT.format(self.table_name))
+                self.__connection.execute(self.__flush_db_statement)
+                self.__connection.execute(self.__table_statement)
                 return True
             except Exception as e:
                 logger.exception("FLUSH_DB command exception")
                 raise e
 
     def __close(self, optimize: bool):
         with self.__lock:
@@ -345,11 +366,11 @@
                 if "expire_time" not in columns:
                     connection.execute(
                         "ALTER TABLE '{}' ADD COLUMN expire_time INTEGER DEFAULT NULL".format(
                             self.table_name
                         )
                     )
             else:
+                connection.execute(self.__table_statement)
 
-                connection.execute(TABLE_STATEMENT.format(self.table_name))
         except Exception:
             logger.exception("Check table error")
```

### Comparing `Kvsqlite-0.2.0.dev0/kvsqlite/sync/client.py` & `Kvsqlite-0.2.1/kvsqlite/sync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         return self.__invoke(request=REQUEST.GET, key=key)
 
     def set(self, key: str, value) -> bool:
         assert isinstance(key, str), "key must be str"
 
         return self.__invoke(request=REQUEST.SET, key=key, value=value)
 
-    def setex(self, key: str, value, ttl: int) -> bool:
+    def setex(self, key: str, ttl: int, value) -> bool:
         assert isinstance(key, str), "key must be str"
         assert ttl >= 1, "ttl must be greater than 1"
 
         return self.__invoke(request=REQUEST.SETEX, key=key, value=[value, ttl])
 
     def delete(self, key: str) -> bool:
         assert isinstance(key, str), "key must be str"
```

### Comparing `Kvsqlite-0.2.0.dev0/setup.py` & `Kvsqlite-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `Kvsqlite-0.2.0.dev0/test/test_kvsqlite.py` & `Kvsqlite-0.2.1/test/test_kvsqlite.py`

 * *Files identical despite different names*

