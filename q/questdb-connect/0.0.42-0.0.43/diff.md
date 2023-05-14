# Comparing `tmp/questdb-connect-0.0.42.tar.gz` & `tmp/questdb-connect-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.42.tar", last modified: Fri May 12 10:34:20 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.43.tar", last modified: Sun May 14 09:22:27 2023, max compression
```

## Comparing `questdb-connect-0.0.42.tar` & `questdb-connect-0.0.43.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.848903 questdb-connect-0.0.42/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.42/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3442 2023-05-12 10:34:20.848765 questdb-connect-0.0.42/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2735 2023-05-10 11:01:02.000000 questdb-connect-0.0.42/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-12 10:33:25.000000 questdb-connect-0.0.42/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-12 10:34:20.848940 questdb-connect-0.0.42/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.843820 questdb-connect-0.0.42/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.845886 questdb-connect-0.0.42/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.42/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.42/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.42/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2785 2023-05-12 10:32:13.000000 questdb-connect-0.0.42/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.42/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.42/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.847016 questdb-connect-0.0.42/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-10 12:28:09.000000 questdb-connect-0.0.42/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.42/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.42/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10966 2023-05-12 10:30:30.000000 questdb-connect-0.0.42/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.42/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.847832 questdb-connect-0.0.42/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3442 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.848491 questdb-connect-0.0.42/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.42/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2563 2023-05-12 10:31:23.000000 questdb-connect-0.0.42/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.42/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.394743 questdb-connect-0.0.43/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.43/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3443 2023-05-14 09:22:27.394602 questdb-connect-0.0.43/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2736 2023-05-13 16:40:56.000000 questdb-connect-0.0.43/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-14 09:21:02.000000 questdb-connect-0.0.43/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-14 09:22:27.394778 questdb-connect-0.0.43/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.389384 questdb-connect-0.0.43/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.391656 questdb-connect-0.0.43/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.43/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.43/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.43/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2785 2023-05-12 10:32:13.000000 questdb-connect-0.0.43/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.43/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.43/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.392770 questdb-connect-0.0.43/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-10 12:28:09.000000 questdb-connect-0.0.43/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.43/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.43/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12644 2023-05-14 09:18:59.000000 questdb-connect-0.0.43/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.43/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.393671 questdb-connect-0.0.43/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3443 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-14 09:22:27.000000 questdb-connect-0.0.43/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-14 09:22:27.394321 questdb-connect-0.0.43/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.43/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4352 2023-05-13 17:16:29.000000 questdb-connect-0.0.43/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.43/tests/test_types.py
```

### Comparing `questdb-connect-0.0.42/LICENSE` & `questdb-connect-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/PKG-INFO` & `questdb-connect-0.0.43/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.42
+Version: 0.0.43
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -64,40 +64,37 @@
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base(metadata=MetaData())
 
 
 class Signal(Base):
     __tablename__ = 'signal'
-    __table_args__ = (qdbc.QDBTableEngine(
-        'signal',
-        'ts',
-        qdbc.PartitionBy.HOUR,
-        is_wal=True),)
+    __table_args__ = (qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True), )
     source = Column(qdbc.Symbol)
     value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
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
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
-please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md).
+please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md)
+if you would like to push a PR.
```

### Comparing `questdb-connect-0.0.42/README.md` & `questdb-connect-0.0.43/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,40 +46,37 @@
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base(metadata=MetaData())
 
 
 class Signal(Base):
     __tablename__ = 'signal'
-    __table_args__ = (qdbc.QDBTableEngine(
-        'signal',
-        'ts',
-        qdbc.PartitionBy.HOUR,
-        is_wal=True),)
+    __table_args__ = (qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True), )
     source = Column(qdbc.Symbol)
     value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
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
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
-please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md).
+please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md)
+if you would like to push a PR.
```

### Comparing `questdb-connect-0.0.42/pyproject.toml` & `questdb-connect-0.0.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.42"
+version = "0.0.43"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.42/src/examples/__init__.py` & `questdb-connect-0.0.43/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/examples/hello_world.py` & `questdb-connect-0.0.43/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.43/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/examples/server_utilisation.py` & `questdb-connect-0.0.43/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.43/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.43/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/questdb_connect/__init__.py` & `questdb-connect-0.0.43/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/questdb_connect/dialect.py` & `questdb-connect-0.0.43/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/questdb_connect/function_names.py` & `questdb-connect-0.0.43/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.43/src/questdb_connect/superset_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
+from flask import current_app
+from flask_babel import gettext as __
+from flask_babel import lazy_gettext as _
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType, TimeGrain
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
@@ -36,27 +39,48 @@
 from .function_names import FUNCTION_NAMES
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
 
+builtin_time_grains: Dict[Optional[str], str] = {
+    "PT1S": __("Second"),
+    "PT5S": __("5 second"),
+    "PT30S": __("30 second"),
+    "PT1M": __("Minute"),
+    "PT5M": __("5 minute"),
+    "PT10M": __("10 minute"),
+    "PT15M": __("15 minute"),
+    "PT30M": __("30 minute"),
+    "PT1H": __("Hour"),
+    "PT6H": __("6 hour"),
+    "P1D": __("Day"),
+    "P1W": __("Week"),
+    "P1M": __("Month"),
+    "P3M": __("Quarter"),
+    "P1Y": __("Year"),
+}
+
+
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = 'questdb'
     engine_name = 'QuestDB Connect'
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
     time_groupby_inline = True
-    allows_hidden_cc_in_orderby=True
+    allows_hidden_cc_in_orderby = True
     time_secondary_columns = True
     max_column_name_length = 120
     try_remove_schema_from_table_name = True
     supports_dynamic_schema = False
     allow_dml = True
+    supports_file_upload = True
+    top_keywords = {}
     _time_grain_expressions = {
         None: '{col}',
         'PT1S': "date_trunc('second', {col})",
         'PT5S': "date_trunc('second', {col}) + 5000000",
         'PT30S': "date_trunc('second', {col}) + 30000000",
         'PT1M': "date_trunc('minute', {col})",
         'PT5M': "date_trunc('minute', {col}) + 300000000",
@@ -118,15 +142,14 @@
     def get_text_clause(cls, clause):
         """SQLAlchemy wrapper to ensure text clauses are escaped properly
         :param clause: string clause with potentially unescaped characters
         :return: text clause with escaped characters
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
-            remove_public_schema(clause)
         return text(remove_public_schema(clause))
 
     @classmethod
     def get_time_grain_expressions(cls) -> Dict[Optional[str], str]:
         """Return a dict of all supported time grains including any
         potential added grains but excluding any potentially disabled
         grains in the config file.
@@ -155,32 +178,54 @@
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
         if type_u in ('DATETIME', 'TIMESTAMP'):
             dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
             return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
     @classmethod
+    def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
+        """Generate a tuple of supported time grains.
+        :return: All time grains supported by the engine
+        """
+        ret_list = []
+        time_grains = builtin_time_grains.copy()
+        time_grains.update(current_app.config["TIME_GRAIN_ADDONS"])
+        for duration, func in cls._time_grain_expressions.items():
+            if duration in time_grains:
+                name = time_grains[duration]
+                ret_list.append(TimeGrain(name, _(name), func, duration))
+        return tuple(ret_list)
+
+    @classmethod
     def get_datatype(cls, type_code: Any) -> Optional[str]:
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
-        return type_code.upper() if isinstance(type_code, str) and type_code else None
+        return type_code.upper() if type_code and isinstance(type_code, str) else 'UNKNOWN'
 
     @classmethod
     def get_column_types(
             cls,
             column_type: Optional[str],
     ) -> Optional[Tuple[TypeEngine, GenericDataType]]:
+        """Return a sqlalchemy native column type and generic data type that
+        corresponds to the column type defined in the data source (return None
+        to use default type inferred by SQLAlchemy). Override `column_type_mappings`
+        for specific needs (see MSSQL for example of NCHAR/NVARCHAR handling).
+        :param column_type: Column type returned by inspector
+        :return: SQLAlchemy and generic Superset column types
+        """
         if not column_type:
             return None
         for regex, sqla_type, generic_type in cls._default_column_type_mappings:
             matching_name = regex.search(column_type)
             if matching_name:
-                return types.resolve_type_from_name(sqla_type.__visit_name__), generic_type
+                qdbcd_type = types.resolve_type_from_name(sqla_type.__visit_name__)
+                return qdbcd_type.impl, generic_type
         return None
 
     @classmethod
     def get_sqla_column_type(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
@@ -190,15 +235,15 @@
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
         if not native_type:
             return None
-        return types.resolve_type_from_name(native_type)
+        return types.resolve_type_from_name(native_type).impl
 
     @classmethod
     def get_column_spec(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
             source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
```

### Comparing `questdb-connect-0.0.42/src/questdb_connect/types.py` & `questdb-connect-0.0.43/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.43/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.42
+Version: 0.0.43
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -64,40 +64,37 @@
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base(metadata=MetaData())
 
 
 class Signal(Base):
     __tablename__ = 'signal'
-    __table_args__ = (qdbc.QDBTableEngine(
-        'signal',
-        'ts',
-        qdbc.PartitionBy.HOUR,
-        is_wal=True),)
+    __table_args__ = (qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True), )
     source = Column(qdbc.Symbol)
     value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
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
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
-please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md).
+please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md)
+if you would like to push a PR.
```

### Comparing `questdb-connect-0.0.42/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.43/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/tests/test_dialect.py` & `questdb-connect-0.0.43/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.42/tests/test_types.py` & `questdb-connect-0.0.43/tests/test_types.py`

 * *Files identical despite different names*

