# Comparing `tmp/ardilla-0.0.8a0.tar.gz` & `tmp/ardilla-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.0.8a0.tar", last modified: Sun May 14 03:17:06 2023, max compression
+gzip compressed data, was "ardilla-0.0.9a0.tar", last modified: Sun May 14 03:47:37 2023, max compression
```

## Comparing `ardilla-0.0.8a0.tar` & `ardilla-0.0.9a0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.548158 ardilla-0.0.8a0/
--rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.8a0/LICENCE
--rw-rw-rw-   0        0        0     4317 2023-05-14 03:17:06.546159 ardilla-0.0.8a0/PKG-INFO
--rw-rw-rw-   0        0        0     3488 2023-05-14 03:10:46.000000 ardilla-0.0.8a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.469050 ardilla-0.0.8a0/ardilla/
--rw-rw-rw-   0        0        0      136 2023-05-13 16:32:48.000000 ardilla-0.0.8a0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     3223 2023-05-14 02:51:15.000000 ardilla-0.0.8a0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.530065 ardilla-0.0.8a0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.8a0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.0.8a0/ardilla/asyncio/abc.py
--rw-rw-rw-   0        0        0     6519 2023-05-14 02:47:39.000000 ardilla-0.0.8a0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     1292 2023-05-13 16:09:59.000000 ardilla-0.0.8a0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     6957 2023-05-14 02:41:42.000000 ardilla-0.0.8a0/ardilla/crud.py
--rw-rw-rw-   0        0        0     1661 2023-05-13 16:03:58.000000 ardilla-0.0.8a0/ardilla/engine.py
--rw-rw-rw-   0        0        0      294 2023-05-13 22:19:12.000000 ardilla-0.0.8a0/ardilla/errors.py
--rw-rw-rw-   0        0        0      217 2023-05-13 16:26:28.000000 ardilla-0.0.8a0/ardilla/logging.py
--rw-rw-rw-   0        0        0     1686 2023-05-13 22:01:58.000000 ardilla-0.0.8a0/ardilla/models.py
--rw-rw-rw-   0        0        0     2153 2023-05-13 22:00:57.000000 ardilla-0.0.8a0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.516048 ardilla-0.0.8a0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     4317 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1047 2023-05-14 03:16:32.000000 ardilla-0.0.8a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 03:17:06.548158 ardilla-0.0.8a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.542064 ardilla-0.0.8a0/tests/
--rw-rw-rw-   0        0        0     5748 2023-05-14 02:49:39.000000 ardilla-0.0.8a0/tests/test_async.py
--rw-rw-rw-   0        0        0      567 2023-05-12 03:32:46.000000 ardilla-0.0.8a0/tests/test_models.py
--rw-rw-rw-   0        0        0     5491 2023-05-14 02:45:01.000000 ardilla-0.0.8a0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.170175 ardilla-0.0.9a0/
+-rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.9a0/LICENCE
+-rw-rw-rw-   0        0        0     4317 2023-05-14 03:47:37.168179 ardilla-0.0.9a0/PKG-INFO
+-rw-rw-rw-   0        0        0     3488 2023-05-14 03:10:46.000000 ardilla-0.0.9a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.064632 ardilla-0.0.9a0/ardilla/
+-rw-rw-rw-   0        0        0      136 2023-05-13 16:32:48.000000 ardilla-0.0.9a0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     3223 2023-05-14 02:51:15.000000 ardilla-0.0.9a0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.151177 ardilla-0.0.9a0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.9a0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.0.9a0/ardilla/asyncio/abc.py
+-rw-rw-rw-   0        0        0     4960 2023-05-14 03:45:11.000000 ardilla-0.0.9a0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0     1292 2023-05-13 16:09:59.000000 ardilla-0.0.9a0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     4754 2023-05-14 03:42:44.000000 ardilla-0.0.9a0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     1661 2023-05-13 16:03:58.000000 ardilla-0.0.9a0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      294 2023-05-13 22:19:12.000000 ardilla-0.0.9a0/ardilla/errors.py
+-rw-rw-rw-   0        0        0      217 2023-05-13 16:26:28.000000 ardilla-0.0.9a0/ardilla/logging.py
+-rw-rw-rw-   0        0        0     1686 2023-05-13 22:01:58.000000 ardilla-0.0.9a0/ardilla/models.py
+-rw-rw-rw-   0        0        0     3106 2023-05-14 03:42:51.000000 ardilla-0.0.9a0/ardilla/queries.py
+-rw-rw-rw-   0        0        0     2153 2023-05-13 22:00:57.000000 ardilla-0.0.9a0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.134195 ardilla-0.0.9a0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     4317 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1047 2023-05-14 03:46:32.000000 ardilla-0.0.9a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 03:47:37.170175 ardilla-0.0.9a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.164178 ardilla-0.0.9a0/tests/
+-rw-rw-rw-   0        0        0     5748 2023-05-14 02:49:39.000000 ardilla-0.0.9a0/tests/test_async.py
+-rw-rw-rw-   0        0        0      567 2023-05-12 03:32:46.000000 ardilla-0.0.9a0/tests/test_models.py
+-rw-rw-rw-   0        0        0     5491 2023-05-14 02:45:01.000000 ardilla-0.0.9a0/tests/test_sync.py
```

### Comparing `ardilla-0.0.8a0/LICENCE` & `ardilla-0.0.9a0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/PKG-INFO` & `ardilla-0.0.9a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ardilla-0.0.8a0/README.md` & `ardilla-0.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/ardilla/abc.py` & `ardilla-0.0.9a0/ardilla/abc.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/ardilla/asyncio/crud.py` & `ardilla-0.0.9a0/ardilla/crud.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,166 +1,131 @@
+import sqlite3
+from sqlite3 import Row
 from typing import Literal, Generic, Self
 
-import aiosqlite
-from aiosqlite import Row
+from .abc import CrudABC, AbstractEngine
+from .models import M, Model as BaseModel
+from .errors import BadQueryError, QueryExecutionError
+from . import queries
 
-from ..errors import BadQueryError, QueryExecutionError
-from ..models import M
-from ..abc import CrudABC
-from ..logging import log, log_query
-
-from .abc import AbstractAsyncEngine
-
-class AsyncCrud(CrudABC, Generic[M]):
+class Crud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
 
-    engine: AbstractAsyncEngine
+    engine: AbstractEngine
 
-    async def _get_or_none_any(self, many: bool, **kws) -> list[M] | M | None:
+    def _get_or_none_any(self, many: bool, **kws) -> list[M] | M | None:
         """
         private helper to the get_or_none queries.
         if param "many" is true it will return a list of matches else will return only one record
         """
-        keys, vals = zip(*kws.items())
-        to_match = f" AND ".join(f"{k} = ?" for k in keys)
-
-        limit = "LIMIT 1;" if not many else ";"
-        q = f"SELECT rowid, * FROM {self.tablename} WHERE ({to_match}) {limit}"
-        log_query(q, vals)
-        async with self.engine as con:
-            async with con.execute(q, vals) as cur:
+        q, vals = queries.for_get_or_none_any(self.tablename, many, kws)
+        with self.engine as con:
+            with self.engine.cursor(con) as cur:
+                cur: sqlite3.Cursor
+                cur.execute(q, vals)
                 if many:
-                    rows: list[Row] = await cur.fetchall()
+                    rows: list[Row] = cur.fetchall()
                     return [self._row2obj(row) for row in rows]
-
                 else:
-                    row: Row | None = await cur.fetchone()
+                    row: Row | None = cur.fetchone()
                     if row:
                         return self._row2obj(row)
-        return
 
-    async def get_or_none(self, **kws) -> M | None:
-        """Gets an object from a database or None if not found"""
-        return await self._get_or_none_any(many=False, **kws)
+    def _do_insert(
+        self, ignore: bool = False, returning: bool = True, /, **kws
+    ) -> M | None:
+        q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
+
+        with self.engine as con:
+            with self.engine.cursor(con) as cur:
+                cur: sqlite3.Cursor
+                try:
+                    cur.execute(q, vals)
+                except sqlite3.IntegrityError as e:
+                    raise QueryExecutionError(str(e))
 
-    async def _do_insert(self, ignore: bool = False, returning: bool = True, /, **kws):
-        keys, vals = zip(*kws.items())
-        placeholders = ", ".join("?" * len(keys))
-        cols = ", ".join(keys)
-
-        q = "INSERT OR IGNORE " if ignore else "INSERT "
-        q += f"INTO {self.tablename} ({cols}) VALUES ({placeholders})"
-        q += " RETURNING *;" if returning else ";"
-        log_query(q, vals)
-        async with self.engine as con:
-            con = await self.engine.connect()
-            cur = None
-            try:
-                cur = await con.execute(q, vals)
-            except aiosqlite.IntegrityError as e:
-                raise QueryExecutionError(str(e))
-            else:
-                row = await cur.fetchone()
-                await con.commit()
+                row = cur.fetchone()
+                con.commit()
                 if returning and row:
                     return self._row2obj(row, cur.lastrowid)
-            finally:
-                if cur is not None:
-                    await cur.close()
-                await con.close()
 
-    async def insert(self, **kws):
+    def get_or_none(self, **kws) -> M | None:
+        """Gets an object from a database or None if not found"""
+        return self._get_or_none_any(many=False, **kws)
+
+    def insert(self, **kws):
         """
         Inserts a record into the database.
         Returns:
             Model | None: Returns a model only if newly created
         Rises:
             ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
         """
-        return await self._do_insert(False, True, **kws)
+        return self._do_insert(False, True, **kws)
 
-    async def insert_or_ignore(self, **kws) -> M | None:
+    def insert_or_ignore(self, **kws) -> M | None:
         """inserts a the object of a row or ignores it if it already exists"""
-        return await self._do_insert(True, True, **kws)
+        return self._do_insert(True, True, **kws)
 
-    async def get_or_create(self, **kws) -> tuple[M, bool]:
+    def get_or_create(self, **kws) -> tuple[M, bool]:
         """Returns object and bool indicated if it was created or not"""
         created = False
-        result = await self.get_or_none(**kws)
+        result = self.get_or_none(**kws)
         if not result:
-            result = await self.insert_or_ignore(**kws)
+            result = self.insert_or_ignore(**kws)
             created = True
         return result, created
 
-    async def get_all(self) -> list[M]:
+    def get_all(self) -> list[M]:
         """Gets all objects from the database"""
-        async with self.engine as con:
-            async with con.execute(f"SELECT rowid, * FROM {self.tablename};") as cur:
-                return [self._row2obj(row) for row in await cur.fetchall()]
+        q = f"SELECT rowid, * FROM {self.tablename};"
+        with self.engine as con:
+            with self.engine.cursor(con) as cur:
+                cur: sqlite3.Cursor
+                cur.execute(q)
+                results: list[Row] = cur.fetchall()
+                return [self._row2obj(res) for res in results]
+            
 
-    async def get_many(self, **kws) -> list[M]:
+    def get_many(self, **kws) -> list[M]:
         """Returns a list of objects that have the given conditions"""
-        return await self._get_or_none_any(many=True, **kws)
+        return self._get_or_none_any(many=True, **kws)
 
-    async def save_one(self, obj: M) -> Literal[True]:
+    def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database"""
-        cols, vals = zip(*obj.dict().items())
-        placeholders = ", ".join("?" * len(cols))
-
-        q = f"""
-        INSERT OR REPLACE INTO {self.tablename} ({', '.join(cols)}) VALUES ({placeholders});
-        """
-        log_query(q, vals)
-        async with self.engine as con:
-            await con.execute(q, vals)
-            await con.commit()
+        q, vals = queries.for_save_one(obj)
+        with self.engine as con:
+            con.execute(q, vals)
+            con.commit()
         return True
 
-    async def save_many(self, *objs: M) -> Literal[True]:
+    def save_many(self, *objs: M) -> Literal[True]:
         """Saves all the given objects to the database"""
-        placeholders = ", ".join("?" * len(self.columns))
-        q = f'INSERT OR REPLACE INTO {self.tablename} ({", ".join(self.columns)}) VALUES ({placeholders});'
-        vals = [tuple(obj.dict().values()) for obj in objs]
-        log_query(q, vals)
-        async with self.engine as con:
-            await con.executemany(q, vals)
-            await con.commit()
+        q, vals = queries.for_save_many(objs)
+        with self.engine as con:
+            con.executemany(q, vals)
+            con.commit()
 
         return True
 
-    async def delete_one(self, obj: M) -> Literal[True]:
+    def delete_one(self, obj: M) -> Literal[True]:
         """
         Deletes the object from the database (won't delete the actual object)
-        queries only by the Model id fields (fields suffixed with 'id')
+        If the object has a PK field or the rowid setup, those will be 
+        used to locate the obj and delete it. 
+        If not, this function will delete any object like this one.
         """
-        obj_dict = obj.dict()
-        id_cols = tuple([k for k in obj_dict if "id" in k])
-        placeholders = ", ".join(f"{k} = ?" for k in id_cols)
-        vals = tuple([obj_dict[k] for k in id_cols])
-        q = f"DELETE FROM {self.tablename} WHERE ({placeholders});"
-        log_query(q, vals)
-        async with self.engine as con:
-            await con.execute(q, vals)
-            await con.commit()
+        
+        q, vals = queries.for_delete_one(obj)
+        with self.engine as con:
+            con.execute(q, vals)
+            con.commit()
+
         return True
 
-    async def delete_many(self, *objs: M) -> Literal[True]:
-        if not objs:
-            raise IndexError('param "objs" is empty, pass at least one object')
-
-        placeholders = ', '.join('?' for _ in objs)
-        if all(obj.__rowid__ for obj in objs):
-            vals = [obj.__rowid__ for obj in objs]    
-            q = f'DELETE FROM {self.tablename} WHERE rowid IN ({placeholders})'
-
-        elif pk := self.Model.__pk__:
-            vals = [getattr(obj, pk) for obj in objs]
-            q = f'DELETE FROM {self.tablename} WHERE id IN ({placeholders})'
-            
-        else:
-            raise BadQueryError('Objects requiere either a primary key or the rowid set for mass deletion')
-        
-        async with self.engine as con:
-            await con.execute(q, vals)
-            await con.commit()
+    def delete_many(self, *objs: M) -> Literal[True]:
+        q, vals = queries.for_delete_many(objs)
+        with self.engine as con:
+            con.execute(q, vals)
+            con.commit()
 
-        return 
+        return True
```

### Comparing `ardilla-0.0.8a0/ardilla/asyncio/engine.py` & `ardilla-0.0.9a0/ardilla/asyncio/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/ardilla/engine.py` & `ardilla-0.0.9a0/ardilla/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/ardilla/models.py` & `ardilla-0.0.9a0/ardilla/models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/ardilla/schemas.py` & `ardilla-0.0.9a0/ardilla/schemas.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/ardilla.egg-info/PKG-INFO` & `ardilla-0.0.9a0/ardilla.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ardilla-0.0.8a0/pyproject.toml` & `ardilla-0.0.9a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.0.8-alpha"
+version = "0.0.9-alpha"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ardilla-0.0.8a0/tests/test_async.py` & `ardilla-0.0.9a0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/tests/test_models.py` & `ardilla-0.0.9a0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.8a0/tests/test_sync.py` & `ardilla-0.0.9a0/tests/test_sync.py`

 * *Files identical despite different names*

