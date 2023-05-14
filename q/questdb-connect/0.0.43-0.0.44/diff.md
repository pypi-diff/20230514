# Comparing `tmp/questdb-connect-0.0.43.tar.gz` & `tmp/questdb-connect-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.43.tar", last modified: Sun May 14 09:22:27 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.44.tar", last modified: Sun May 14 12:46:48 2023, max compression
```

## Comparing `questdb-connect-0.0.43.tar` & `questdb-connect-0.0.44.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.394743 questdb-connect-0.0.43/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.43/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3443 2023-05-14 09:22:27.394602 questdb-connect-0.0.43/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2736 2023-05-13 16:40:56.000000 questdb-connect-0.0.43/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-14 09:21:02.000000 questdb-connect-0.0.43/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-14 09:22:27.394778 questdb-connect-0.0.43/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.389384 questdb-connect-0.0.43/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.391656 questdb-connect-0.0.43/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.43/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.43/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.43/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2785 2023-05-12 10:32:13.000000 questdb-connect-0.0.43/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.43/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.43/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.392770 questdb-connect-0.0.43/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-10 12:28:09.000000 questdb-connect-0.0.43/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.43/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.43/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12644 2023-05-14 09:18:59.000000 questdb-connect-0.0.43/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.43/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.393671 questdb-connect-0.0.43/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3443 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.394321 questdb-connect-0.0.43/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.43/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4352 2023-05-13 17:16:29.000000 questdb-connect-0.0.43/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.43/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.919501 questdb-connect-0.0.44/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.44/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-14 12:46:48.919367 questdb-connect-0.0.44/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.44/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-14 12:44:33.000000 questdb-connect-0.0.44/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-14 12:46:48.921581 questdb-connect-0.0.44/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.913295 questdb-connect-0.0.44/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.915407 questdb-connect-0.0.44/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.44/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.44/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.44/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2839 2023-05-14 10:10:59.000000 questdb-connect-0.0.44/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.44/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.44/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.916976 questdb-connect-0.0.44/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-14 09:35:51.000000 questdb-connect-0.0.44/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.44/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.44/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11549 2023-05-14 12:43:14.000000 questdb-connect-0.0.44/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.44/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.918223 questdb-connect-0.0.44/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-14 12:46:48.000000 questdb-connect-0.0.44/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 12:46:48.918969 questdb-connect-0.0.44/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.44/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4352 2023-05-13 17:16:29.000000 questdb-connect-0.0.44/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.44/tests/test_types.py
```

### Comparing `questdb-connect-0.0.43/LICENSE` & `questdb-connect-0.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/PKG-INFO` & `questdb-connect-0.0.44/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.43
+Version: 0.0.44
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -76,16 +76,16 @@
 
 def main():
     engine = create_engine('questdb://localhost:8812/main')
     try:
         Base.metadata.create_all(engine)
         with engine.connect() as conn:
             conn.execute(insert(Signal).values(
-                source='coconut', 
-                value=16.88993244, 
+                source='coconut',
+                value=16.88993244,
                 ts=datetime.datetime.utcnow()
             ))
     finally:
         if engine:
             engine.dispose()
```

### Comparing `questdb-connect-0.0.43/README.md` & `questdb-connect-0.0.44/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
 def main():
     engine = create_engine('questdb://localhost:8812/main')
     try:
         Base.metadata.create_all(engine)
         with engine.connect() as conn:
             conn.execute(insert(Signal).values(
-                source='coconut', 
-                value=16.88993244, 
+                source='coconut',
+                value=16.88993244,
                 ts=datetime.datetime.utcnow()
             ))
     finally:
         if engine:
             engine.dispose()
```

### Comparing `questdb-connect-0.0.43/pyproject.toml` & `questdb-connect-0.0.44/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -18,33 +18,33 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
-name = "questdb-connect"
-version = "0.0.43"
-authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
+name = 'questdb-connect'
+version = '0.0.44'
+authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
 dependencies = []
 
 [project.urls]
-"Homepage" = "https://github.com/questdb/questdb-connect/"
-"Bug Tracker" = "https://github.com/questdb/questdb-connect/issues/"
+'Homepage' = "https://github.com/questdb/questdb-connect/"
+'Bug Tracker' = "https://github.com/questdb/questdb-connect/issues/"
 
 [project.entry-points.'sqlalchemy.dialects']
 questdb = 'questdb_connect.dialect:QuestDBDialect'
 
 [project.entry-points.'superset.db_engine_specs']
 questdb = 'questdb_connect.superset:QDBEngineSpec'
 
@@ -72,13 +72,13 @@
 ]
 
 [tool.ruff.pylint]
 max-branches = 20
 max-args = 10
 
 [tool.ruff.per-file-ignores]
-"tests/test_dialect.py" = ["S101"]
-"tests/test_types.py" = ["S101"]
-"tests/test_superset.py" = ["S101"]
-"tests/conftest.py" = ["S608"]
-"src/examples/sqlalchemy_raw.py" = ["S608"]
-"src/examples/server_utilisation.py" = ["S311"]
+'tests/test_dialect.py' = ['S101']
+'tests/test_types.py' = ['S101']
+'tests/test_superset.py' = ['S101']
+'tests/conftest.py' = ['S608']
+'src/examples/sqlalchemy_raw.py' = ['S608']
+'src/examples/server_utilisation.py' = ['S311']
```

### Comparing `questdb-connect-0.0.43/src/examples/__init__.py` & `questdb-connect-0.0.44/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/src/examples/hello_world.py` & `questdb-connect-0.0.44/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.44/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/src/examples/server_utilisation.py` & `questdb-connect-0.0.44/src/examples/server_utilisation.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,19 +74,20 @@
     session = Session(engine)
     max_batch_size = 3000
     try:
         Base.metadata.drop_all(engine)
         Base.metadata.create_all(engine)
         batch_size = 0
         while time.time() < end_time:
+            node = Nodes.rand()
             session.add(
                 NodeMetrics(
-                    source=Nodes.rand().name,
+                    source=node.name,
                     attr_name=Metrics.rand().name,
-                    attr_value=random.random() * 100.0,
+                    attr_value=random.random() * node.value * random.randint(1, 100),
                     ts=datetime.datetime.utcnow()
                 )
             )
             batch_size += 1
             if batch_size > max_batch_size:
                 session.commit()
                 batch_size = 0
```

### Comparing `questdb-connect-0.0.43/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.44/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.44/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/src/questdb_connect/__init__.py` & `questdb-connect-0.0.44/src/questdb_connect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 #  limitations under the License.
 #
 import re
 
 import psycopg2
 
 # ===== DBAPI =====
-
 # https://peps.python.org/pep-0249/
 
 apilevel = '2.0'
 threadsafety = 2
 paramstyle = 'pyformat'
 public_schema_filter = re.compile(r"(')?(public(?(1)\1|)\.)", re.IGNORECASE | re.MULTILINE)
```

### Comparing `questdb-connect-0.0.43/src/questdb_connect/dialect.py` & `questdb-connect-0.0.44/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/src/questdb_connect/function_names.py` & `questdb-connect-0.0.44/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.44/src/questdb_connect/superset_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
-from flask import current_app
-from flask_babel import gettext as __
-from flask_babel import lazy_gettext as _
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType, TimeGrain
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
@@ -39,33 +36,14 @@
 from .function_names import FUNCTION_NAMES
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
 
-builtin_time_grains: Dict[Optional[str], str] = {
-    "PT1S": __("Second"),
-    "PT5S": __("5 second"),
-    "PT30S": __("30 second"),
-    "PT1M": __("Minute"),
-    "PT5M": __("5 minute"),
-    "PT10M": __("10 minute"),
-    "PT15M": __("15 minute"),
-    "PT30M": __("30 minute"),
-    "PT1H": __("Hour"),
-    "PT6H": __("6 hour"),
-    "P1D": __("Day"),
-    "P1W": __("Week"),
-    "P1M": __("Month"),
-    "P3M": __("Quarter"),
-    "P1Y": __("Year"),
-}
-
-
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = 'questdb'
     engine_name = 'QuestDB Connect'
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
     time_groupby_inline = True
@@ -108,14 +86,15 @@
         (re.compile("^STRING", re.IGNORECASE), types.String, GenericDataType.STRING),
         (re.compile("^UUID", re.IGNORECASE), types.UUID, GenericDataType.STRING),
         (re.compile("^CHAR", re.IGNORECASE), types.Char, GenericDataType.STRING),
         (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp, GenericDataType.TEMPORAL),
         (re.compile("^DATE", re.IGNORECASE), types.Date, GenericDataType.TEMPORAL),
         (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), types.GeohashLong, GenericDataType.STRING),
     )
+    column_type_mappings = _default_column_type_mappings
 
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
     ) -> str:
@@ -178,28 +157,14 @@
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
         if type_u in ('DATETIME', 'TIMESTAMP'):
             dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
             return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
     @classmethod
-    def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
-        """Generate a tuple of supported time grains.
-        :return: All time grains supported by the engine
-        """
-        ret_list = []
-        time_grains = builtin_time_grains.copy()
-        time_grains.update(current_app.config["TIME_GRAIN_ADDONS"])
-        for duration, func in cls._time_grain_expressions.items():
-            if duration in time_grains:
-                name = time_grains[duration]
-                ret_list.append(TimeGrain(name, _(name), func, duration))
-        return tuple(ret_list)
-
-    @classmethod
     def get_datatype(cls, type_code: Any) -> Optional[str]:
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
         return type_code.upper() if type_code and isinstance(type_code, str) else 'UNKNOWN'
```

### Comparing `questdb-connect-0.0.43/src/questdb_connect/types.py` & `questdb-connect-0.0.44/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.44/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.43
+Version: 0.0.44
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -76,16 +76,16 @@
 
 def main():
     engine = create_engine('questdb://localhost:8812/main')
     try:
         Base.metadata.create_all(engine)
         with engine.connect() as conn:
             conn.execute(insert(Signal).values(
-                source='coconut', 
-                value=16.88993244, 
+                source='coconut',
+                value=16.88993244,
                 ts=datetime.datetime.utcnow()
             ))
     finally:
         if engine:
             engine.dispose()
```

### Comparing `questdb-connect-0.0.43/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.44/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/tests/test_dialect.py` & `questdb-connect-0.0.44/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/tests/test_superset.py` & `questdb-connect-0.0.44/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.43/tests/test_types.py` & `questdb-connect-0.0.44/tests/test_types.py`

 * *Files identical despite different names*

