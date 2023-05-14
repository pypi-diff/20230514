# Comparing `tmp/ardilla-0.0.7a0.tar.gz` & `tmp/ardilla-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.0.7a0.tar", last modified: Sat May 13 17:33:54 2023, max compression
+gzip compressed data, was "ardilla-0.0.8a0.tar", last modified: Sun May 14 03:17:06 2023, max compression
```

## Comparing `ardilla-0.0.7a0.tar` & `ardilla-0.0.8a0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 17:33:54.541981 ardilla-0.0.7a0/
--rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.7a0/LICENCE
--rw-rw-rw-   0        0        0     3988 2023-05-13 17:33:54.536979 ardilla-0.0.7a0/PKG-INFO
--rw-rw-rw-   0        0        0     3297 2023-05-12 03:38:21.000000 ardilla-0.0.7a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 17:33:54.458981 ardilla-0.0.7a0/ardilla/
--rw-rw-rw-   0        0        0      136 2023-05-13 16:32:48.000000 ardilla-0.0.7a0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     3240 2023-05-13 04:14:16.000000 ardilla-0.0.7a0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:33:54.515978 ardilla-0.0.7a0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.7a0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.0.7a0/ardilla/asyncio/abc.py
--rw-rw-rw-   0        0        0     6364 2023-05-13 16:27:36.000000 ardilla-0.0.7a0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     1292 2023-05-13 16:09:59.000000 ardilla-0.0.7a0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     6753 2023-05-13 04:30:42.000000 ardilla-0.0.7a0/ardilla/crud.py
--rw-rw-rw-   0        0        0     1661 2023-05-13 16:03:58.000000 ardilla-0.0.7a0/ardilla/engine.py
--rw-rw-rw-   0        0        0      216 2023-05-11 02:46:57.000000 ardilla-0.0.7a0/ardilla/errors.py
--rw-rw-rw-   0        0        0      217 2023-05-13 16:26:28.000000 ardilla-0.0.7a0/ardilla/logging.py
--rw-rw-rw-   0        0        0     1475 2023-05-12 03:30:34.000000 ardilla-0.0.7a0/ardilla/models.py
--rw-rw-rw-   0        0        0     2151 2023-05-13 04:07:51.000000 ardilla-0.0.7a0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:33:54.499980 ardilla-0.0.7a0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     3988 2023-05-13 17:33:54.000000 ardilla-0.0.7a0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-05-13 17:33:54.000000 ardilla-0.0.7a0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 17:33:54.000000 ardilla-0.0.7a0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-05-13 17:33:54.000000 ardilla-0.0.7a0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-13 17:33:54.000000 ardilla-0.0.7a0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      916 2023-05-13 17:32:31.000000 ardilla-0.0.7a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 17:33:54.542976 ardilla-0.0.7a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 17:33:54.531976 ardilla-0.0.7a0/tests/
--rw-rw-rw-   0        0        0     5291 2023-05-12 03:30:55.000000 ardilla-0.0.7a0/tests/test_async.py
--rw-rw-rw-   0        0        0      567 2023-05-12 03:32:46.000000 ardilla-0.0.7a0/tests/test_models.py
--rw-rw-rw-   0        0        0     4964 2023-05-12 03:31:02.000000 ardilla-0.0.7a0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.548158 ardilla-0.0.8a0/
+-rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.8a0/LICENCE
+-rw-rw-rw-   0        0        0     4317 2023-05-14 03:17:06.546159 ardilla-0.0.8a0/PKG-INFO
+-rw-rw-rw-   0        0        0     3488 2023-05-14 03:10:46.000000 ardilla-0.0.8a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.469050 ardilla-0.0.8a0/ardilla/
+-rw-rw-rw-   0        0        0      136 2023-05-13 16:32:48.000000 ardilla-0.0.8a0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     3223 2023-05-14 02:51:15.000000 ardilla-0.0.8a0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.530065 ardilla-0.0.8a0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.8a0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.0.8a0/ardilla/asyncio/abc.py
+-rw-rw-rw-   0        0        0     6519 2023-05-14 02:47:39.000000 ardilla-0.0.8a0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0     1292 2023-05-13 16:09:59.000000 ardilla-0.0.8a0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     6957 2023-05-14 02:41:42.000000 ardilla-0.0.8a0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     1661 2023-05-13 16:03:58.000000 ardilla-0.0.8a0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      294 2023-05-13 22:19:12.000000 ardilla-0.0.8a0/ardilla/errors.py
+-rw-rw-rw-   0        0        0      217 2023-05-13 16:26:28.000000 ardilla-0.0.8a0/ardilla/logging.py
+-rw-rw-rw-   0        0        0     1686 2023-05-13 22:01:58.000000 ardilla-0.0.8a0/ardilla/models.py
+-rw-rw-rw-   0        0        0     2153 2023-05-13 22:00:57.000000 ardilla-0.0.8a0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.516048 ardilla-0.0.8a0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     4317 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 03:17:06.000000 ardilla-0.0.8a0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1047 2023-05-14 03:16:32.000000 ardilla-0.0.8a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 03:17:06.548158 ardilla-0.0.8a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 03:17:06.542064 ardilla-0.0.8a0/tests/
+-rw-rw-rw-   0        0        0     5748 2023-05-14 02:49:39.000000 ardilla-0.0.8a0/tests/test_async.py
+-rw-rw-rw-   0        0        0      567 2023-05-12 03:32:46.000000 ardilla-0.0.8a0/tests/test_models.py
+-rw-rw-rw-   0        0        0     5491 2023-05-14 02:45:01.000000 ardilla-0.0.8a0/tests/test_sync.py
```

### Comparing `ardilla-0.0.7a0/LICENCE` & `ardilla-0.0.8a0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.7a0/PKG-INFO` & `ardilla-0.0.8a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.7a0
-Summary: A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic
+Version: 0.0.8a0
+Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: examples
 Provides-Extra: dev
 License-File: LICENCE
 
 # ardilla
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
```

### Comparing `ardilla-0.0.7a0/README.md` & `ardilla-0.0.8a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # ardilla
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
```

### Comparing `ardilla-0.0.7a0/ardilla/abc.py` & `ardilla-0.0.8a0/ardilla/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     def _row2obj(self, row: Row, rowid: int = None) -> M:
         """
         Args:
             row: the sqlite row
             rowid: the rowid of the row.
                 If passed it means it comes from an insert function
-                meaning the rowid
+                
         """
         [*keys] = self.Model.__fields__
         if rowid is None:
             rowid, *vals = row
         else:
             vals = list(row)
         data = {k: v for k, v in zip(keys, vals)}
```

### Comparing `ardilla-0.0.7a0/ardilla/asyncio/crud.py` & `ardilla-0.0.8a0/ardilla/asyncio/crud.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Literal, Generic, Self
 
 import aiosqlite
 from aiosqlite import Row
 
-from ..errors import QueryExecutionError
+from ..errors import BadQueryError, QueryExecutionError
 from ..models import M
 from ..abc import CrudABC
 from ..logging import log, log_query
 
 from .abc import AbstractAsyncEngine
 
 class AsyncCrud(CrudABC, Generic[M]):
@@ -90,16 +90,16 @@
             result = await self.insert_or_ignore(**kws)
             created = True
         return result, created
 
     async def get_all(self) -> list[M]:
         """Gets all objects from the database"""
         async with self.engine as con:
-            async with con.execute(f"SELECT * FROM {self.tablename};") as cur:
-                return [self.Model(**row) for row in await cur.fetchall()]
+            async with con.execute(f"SELECT rowid, * FROM {self.tablename};") as cur:
+                return [self._row2obj(row) for row in await cur.fetchall()]
 
     async def get_many(self, **kws) -> list[M]:
         """Returns a list of objects that have the given conditions"""
         return await self._get_or_none_any(many=True, **kws)
 
     async def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database"""
@@ -143,23 +143,24 @@
             await con.commit()
         return True
 
     async def delete_many(self, *objs: M) -> Literal[True]:
         if not objs:
             raise IndexError('param "objs" is empty, pass at least one object')
 
-        prot = objs[0]
-        id_cols = tuple([k for k in prot.dict() if "id" in k])
-        placeholders = " OR ".join(
-            f"({', '.join(f'{k} = ?' for k in id_cols)})" for _ in objs
-        )
-        vals = tuple(
-            [val for obj in objs for key, val in obj.dict().items() if key in id_cols]
-        )
-
-        q = f"DELETE FROM {self.tablename} WHERE {placeholders};"
-        log_query(q, vals)
+        placeholders = ', '.join('?' for _ in objs)
+        if all(obj.__rowid__ for obj in objs):
+            vals = [obj.__rowid__ for obj in objs]    
+            q = f'DELETE FROM {self.tablename} WHERE rowid IN ({placeholders})'
+
+        elif pk := self.Model.__pk__:
+            vals = [getattr(obj, pk) for obj in objs]
+            q = f'DELETE FROM {self.tablename} WHERE id IN ({placeholders})'
+            
+        else:
+            raise BadQueryError('Objects requiere either a primary key or the rowid set for mass deletion')
+        
         async with self.engine as con:
             await con.execute(q, vals)
             await con.commit()
 
         return
```

### Comparing `ardilla-0.0.7a0/ardilla/asyncio/engine.py` & `ardilla-0.0.8a0/ardilla/asyncio/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.7a0/ardilla/crud.py` & `ardilla-0.0.8a0/ardilla/crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 from sqlite3 import Row
 from typing import Literal, Generic, Self
 
 from .abc import CrudABC, AbstractEngine
 from .models import M, Model as BaseModel
-from .errors import QueryExecutionError
+from .errors import BadQueryError, QueryExecutionError
 
 
 class Crud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
 
     engine: AbstractEngine
 
@@ -84,21 +84,22 @@
         if not result:
             result = self.insert_or_ignore(**kws)
             created = True
         return result, created
 
     def get_all(self) -> list[M]:
         """Gets all objects from the database"""
-        q = f"SELECT * FROM {self.tablename};"
+        q = f"SELECT rowid, * FROM {self.tablename};"
         with self.engine as con:
             with self.engine.cursor(con) as cur:
                 cur: sqlite3.Cursor
                 cur.execute(q)
-                results = cur.fetchall()
-                return [self.Model(**res) for res in results]
+                results: list[Row] = cur.fetchall()
+                return [self._row2obj(res) for res in results]
+            
 
     def get_many(self, **kws) -> list[M]:
         """Returns a list of objects that have the given conditions"""
         return self._get_or_none_any(many=True, **kws)
 
     def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database"""
@@ -111,15 +112,14 @@
             vals += obj.__rowid__
 
         else:
             placeholders = ", ".join("?" * len(cols))
             upsert_query = f"""
             INSERT OR REPLACE INTO {self.tablename} ({', '.join(cols)}) VALUES ({placeholders});
             """
-
         with self.engine as con:
             con.execute(upsert_query, vals)
             con.commit()
         return True
 
     def save_many(self, *objs: M) -> Literal[True]:
         """Saves all the given objects to the database"""
@@ -160,23 +160,24 @@
 
         return True
 
     def delete_many(self, *objs: M) -> Literal[True]:
         if not objs:
             raise IndexError('param "objs" is empty, pass at least one object')
 
-        prot = objs[0]
-        id_cols = tuple([k for k in prot.dict() if "id" in k])
-        placeholders = " OR ".join(
-            f"({', '.join(f'{k} = ?' for k in id_cols)})" for _ in objs
-        )
-        vals = tuple(
-            [val for obj in objs for key, val in obj.dict().items() if key in id_cols]
-        )
-
-        q = f"DELETE FROM {self.tablename} WHERE {placeholders};"
-
+        placeholders = ', '.join('?' for _ in objs)
+        if all(obj.__rowid__ for obj in objs):
+            vals = [obj.__rowid__ for obj in objs]    
+            q = f'DELETE FROM {self.tablename} WHERE rowid IN ({placeholders})'
+
+        elif pk := self.Model.__pk__:
+            vals = [getattr(obj, pk) for obj in objs]
+            q = f'DELETE FROM {self.tablename} WHERE id IN ({placeholders})'
+            
+        else:
+            raise BadQueryError('Objects requiere either a primary key or the rowid set for mass deletion')
+        
         with self.engine as con:
             con.execute(q, vals)
             con.commit()
 
         return True
```

### Comparing `ardilla-0.0.7a0/ardilla/engine.py` & `ardilla-0.0.8a0/ardilla/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.7a0/ardilla/models.py` & `ardilla-0.0.8a0/ardilla/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,24 +10,30 @@
     __pk__: str | None  # tells the model which key to idenfity as primary
     __tablename__: str  # will default to the lowercase name of the subclass
     __schema__: str  # best effort will be made if it's missing
     # there's no support for constrains or foreign fields yet but you can
     # define your own schema to support them
 
     def __init_subclass__(cls, **kws) -> None:
+        pk = None
         for field in cls.__fields__.values():
             if field.type_ not in FIELD_MAPPING:
                 raise ModelIntegrityError(
                     f'Field "{field.name}" of model "{cls.__name__}" is of unsupported type "{field.type_}"'
                 )
+            if (
+                field.field_info.extra.get('primary') 
+                or field.field_info.extra.get('primary_key')
+            ):
+                pk = field.name 
 
         if not hasattr(cls, "__schema__"):
             cls.__schema__ = make_schema(cls)
 
-        cls.__pk__ = get_pk(cls.__schema__)
+        cls.__pk__ = pk or get_pk(cls.__schema__)
 
         if not hasattr(cls, "__tablename__"):
             tablename = get_tablename(cls)
             setattr(cls, "__tablename__", tablename)
 
         super().__init_subclass__(**kws)
```

### Comparing `ardilla-0.0.7a0/ardilla/schemas.py` & `ardilla-0.0.8a0/ardilla/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         type_ = FIELD_MAPPING[field.type_]
         pk = getattr(model, "__pk__", None)
         field_is_pk = field.field_info.extra.get(
             "primary"
         ) or field.field_info.extra.get("primary_key")
         if field_is_pk and pk and field.name != pk:
             raise ModelIntegrityError(
-                f"field {field.name} is marked as pk, but __pk__ points to other field."
+                f"field {field.name} is marked as pk, but __pk__ points to another field."
             )
         out = f"    {field.name} {type_}"
         if pk == field.name or field_is_pk:
             out += " PRIMARY KEY"
             if field.field_info.extra.get("autoincrement"):
                 out += " AUTOINCREMENT"
         if field.required and not "PRIMARY KEY" in out:
```

### Comparing `ardilla-0.0.7a0/ardilla.egg-info/PKG-INFO` & `ardilla-0.0.8a0/ardilla.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.7a0
-Summary: A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic
+Version: 0.0.8a0
+Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: examples
 Provides-Extra: dev
 License-File: LICENCE
 
 # ardilla
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
```

### Comparing `ardilla-0.0.7a0/pyproject.toml` & `ardilla-0.0.8a0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.0.7-alpha"
+version = "0.0.8-alpha"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
-description = "A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic"
+description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-  "Programming Language :: Python :: 3",
+  "Intended Audience :: Developers",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Development Status :: 3 - Alpha",
 ]
 dependencies = [
   "pydantic==1.10.7",
 ]
 
 [project.optional-dependencies]
 async = ["aiosqlite==0.19.0",]
 examples = ["fastapi-0.95.1", "uvicorn-0.22.0"]
-dev = ["pytest==7.3.1", "pytest-asyncio==0.21.0", "black==23.3.0"]
+dev = [
+  "pytest==7.3.1", 
+  "pytest-asyncio==0.21.0", 
+  "black==23.3.0"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/chrisdewa/ardilla"
 "Bug Tracker" = "https://github.com/chrisdewa/ardilla/issues"
```

### Comparing `ardilla-0.0.7a0/tests/test_async.py` & `ardilla-0.0.8a0/tests/test_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,19 +155,38 @@
         moni = User(id=2, name="moni", age=36)
         elena = User(id=3, name="elena", age=5)
         await crud.save_many(chris, moni, elena)
         await crud.delete_one(moni)
         users = await crud.get_all()
         assert len(users) == 2, "Delete one didn't delete the correct amount of users"
 
-
 @pytest.mark.asyncio
-async def test_delete_many():
+async def test_delete_many_by_id():
     async with cleanup() as crud:
-        chris = User(id=1, name="chris", age=35)
-        moni = User(id=2, name="moni", age=36)
-        elena = User(id=3, name="elena", age=5)
-        await crud.save_many(chris, moni, elena)
+        users = [
+            User(id=n, name='chris', age=n)
+            for n in range(10)
+        ]
+        await crud.save_many(*users)
+        
+        to_delete = users[:-1]
+        await crud.delete_many(*to_delete)
+        
+        users = await crud.get_all()
+        assert len(users) == 1, "Delete many didn't delete the correct amount of users"
 
-        await crud.delete_many(chris, elena)
+@pytest.mark.asyncio
+async def test_delete_many_by_rowid():
+    async with cleanup() as crud:
+        users = [
+            User(id=n, name='chris', age=n)
+            for n in range(10)
+        ]
+        await crud.save_many(*users)
+       
+        await crud.delete_many(*users[:-1])
+        
         users = await crud.get_all()
+        
+        
         assert len(users) == 1, "Delete many didn't delete the correct amount of users"
+
```

### Comparing `ardilla-0.0.7a0/tests/test_models.py` & `ardilla-0.0.8a0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.7a0/tests/test_sync.py` & `ardilla-0.0.8a0/tests/test_sync.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 path = Path(__file__).parent
 db = path / "testdb.sqlite"
 
 
 class User(Model):
-    id: int = Field(primary=True)
+    id: int = Field(primary=True, autoincrement=True)
     name: str
     age: int
 
 
 @contextmanager
 def cleanup():
     try:
@@ -123,14 +123,15 @@
         u4 = User(id=4, name="moni", age=34)
         u5 = User(id=5, name="fran", age=1)
         crud.save_many(u1, u2, u3, u4, u5)
 
         users = crud.get_many(name="chris")
 
         assert len(users) == 3, "Incorrect number of users returned"
+        assert all(u.__rowid__ for u in users), 'User objects did not get their rowid populated'
 
 
 def test_get_or_create():
     with cleanup() as crud:
         elena = User(id=1, name="elena", age=5)
         crud.save_one(elena)
 
@@ -160,17 +161,37 @@
         elena = User(id=3, name="elena", age=5)
         crud.save_many(chris, moni, elena)
         crud.delete_one(moni)
         users = crud.get_all()
         assert len(users) == 2, "Delete one didn't delete the correct amount of users"
 
 
-def test_delete_many():
+def test_delete_many_by_id():
     with cleanup() as crud:
-        chris = User(id=1, name="chris", age=35)
-        moni = User(id=2, name="moni", age=36)
-        elena = User(id=3, name="elena", age=5)
-        crud.save_many(chris, moni, elena)
+        users = [
+            User(id=n, name='chris', age=n)
+            for n in range(10)
+        ]
+        crud.save_many(*users)
+        
+        to_delete = users[:-1]
+        crud.delete_many(*to_delete)
+        
+        users = crud.get_all()
+        assert len(users) == 1, "Delete many didn't delete the correct amount of users"
+
 
-        crud.delete_many(chris, elena)
+def test_delete_many_by_rowid():
+    with cleanup() as crud:
+        users = [
+            User(id=n, name='chris', age=n)
+            for n in range(10)
+        ]
+        crud.save_many(*users)
+       
+        crud.delete_many(*users[:-1])
+        
         users = crud.get_all()
+        
+        
         assert len(users) == 1, "Delete many didn't delete the correct amount of users"
+
```

