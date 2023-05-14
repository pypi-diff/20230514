# Comparing `tmp/orso-0.0.8.tar.gz` & `tmp/orso-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orso-0.0.8.tar", last modified: Sat Mar 11 00:25:43 2023, max compression
+gzip compressed data, was "orso-0.0.9.tar", last modified: Sun Mar 12 02:47:11 2023, max compression
```

## Comparing `orso-0.0.8.tar` & `orso-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:25:43.823135 orso-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-11 00:25:29.000000 orso-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-11 00:25:43.823135 orso-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-11 00:25:29.000000 orso-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:25:43.819136 orso-0.0.8/orso/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-11 00:25:29.000000 orso-0.0.8/orso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-03-11 00:25:29.000000 orso-0.0.8/orso/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-03-11 00:25:29.000000 orso-0.0.8/orso/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-03-11 00:25:29.000000 orso-0.0.8/orso/display.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-11 00:25:29.000000 orso-0.0.8/orso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-11 00:25:29.000000 orso-0.0.8/orso/row.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-11 00:25:29.000000 orso-0.0.8/orso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:25:43.819136 orso-0.0.8/orso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-11 00:25:43.000000 orso-0.0.8/orso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-11 00:25:43.000000 orso-0.0.8/orso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 00:25:43.000000 orso-0.0.8/orso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-11 00:25:43.000000 orso-0.0.8/orso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-11 00:25:43.000000 orso-0.0.8/orso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-11 00:25:29.000000 orso-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 00:25:43.823135 orso-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-11 00:25:29.000000 orso-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 00:25:43.823135 orso-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-11 00:25:29.000000 orso-0.0.8/tests/test_converters_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-03-11 00:25:29.000000 orso-0.0.8/tests/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-11 00:25:29.000000 orso-0.0.8/tests/test_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-11 00:25:29.000000 orso-0.0.8/tests/test_load_from_pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:47:11.041472 orso-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-03-12 02:46:53.000000 orso-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-12 02:47:11.041472 orso-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-12 02:46:53.000000 orso-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:47:11.037472 orso-0.0.9/orso/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-12 02:46:53.000000 orso-0.0.9/orso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-03-12 02:46:53.000000 orso-0.0.9/orso/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-03-12 02:46:53.000000 orso-0.0.9/orso/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-03-12 02:46:53.000000 orso-0.0.9/orso/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-12 02:46:53.000000 orso-0.0.9/orso/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-12 02:46:53.000000 orso-0.0.9/orso/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-12 02:46:53.000000 orso-0.0.9/orso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:47:11.037472 orso-0.0.9/orso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-12 02:47:11.000000 orso-0.0.9/orso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-12 02:46:53.000000 orso-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 02:47:11.041472 orso-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-12 02:46:53.000000 orso-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:47:11.041472 orso-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-12 02:46:53.000000 orso-0.0.9/tests/test_converters_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-12 02:46:53.000000 orso-0.0.9/tests/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-12 02:46:53.000000 orso-0.0.9/tests/test_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-12 02:46:53.000000 orso-0.0.9/tests/test_load_from_pyarrow.py
```

### Comparing `orso-0.0.8/PKG-INFO` & `orso-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orso
-Version: 0.0.8
+Version: 0.0.9
 Summary: 🐻 Dataframe Library
 Home-page: https://github.com/mabel-dev/orso/
 Author: @joocer
 Author-email: justin.joyce@joocer.com
 Maintainer: @joocer
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,15 +22,17 @@
 
 </div>
 
 Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
 
 ## License
 
-[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mabel-dev/orso/blob/main/LICENSE)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mabel-dev/orso/blob/master/LICENSE)
+
+Orso is licensed under Apache 2.0 unless explicitly indicated otherwise.
 
 ## Status
 
 [![Status](https://img.shields.io/badge/Status-alpha-orange)](https://github.com/mabel-dev/orso)
 
 Orso is in alpha. Alpha means different things to different people, to us, being alpha means:
```

### Comparing `orso-0.0.8/README.md` & `orso-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 </div>
 
 Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
 
 ## License
 
-[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mabel-dev/orso/blob/main/LICENSE)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mabel-dev/orso/blob/master/LICENSE)
+
+Orso is licensed under Apache 2.0 unless explicitly indicated otherwise.
 
 ## Status
 
 [![Status](https://img.shields.io/badge/Status-alpha-orange)](https://github.com/mabel-dev/orso)
 
 Orso is in alpha. Alpha means different things to different people, to us, being alpha means:
```

### Comparing `orso-0.0.8/orso/converters.py` & `orso-0.0.9/orso/converters.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 import typing
 
 from orso.dataframe import DataFrame
 from orso.exceptions import MissingDependencyError
 from orso.row import Row
 
 
-def to_arrow(dataset):
+def to_arrow(dataset, size=None):
     try:
         import pyarrow
     except ImportError as import_error:
         raise MissingDependencyError(import_error.name) from import_error
     # Create a list of PyArrow arrays from the rows
     arrays = [pyarrow.array(col) for col in zip(*dataset._rows)]
+    # Limit the number of rows to 'size'
+    if size:
+        arrays = itertools.islice(arrays, size)
     # Create a PyArrow table from the arrays and schema
     table = pyarrow.Table.from_arrays(arrays, dataset.column_names)
 
     return table
 
 
 def from_arrow(tables, size=None):
```

### Comparing `orso-0.0.8/orso/dataframe.py` & `orso-0.0.9/orso/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,18 +47,18 @@
 
     @classmethod
     def from_arrow(cls, tables):
         from orso.converters import from_arrow
 
         return from_arrow(tables)
 
-    def arrow(self):
+    def arrow(self, size=None):
         from orso.converters import to_arrow
 
-        return to_arrow(self)
+        return to_arrow(self, size=size)
 
     def pandas(self):
         from orso.converters import to_pandas
 
         return to_pandas(self)
 
     def polars(self):
@@ -145,14 +145,20 @@
         self.materialize()
         if offset < 0:
             offset = len(self._rows) + offset
         if length is None:
             return DataFrame(schema=self._schema, rows=self._rows[offset:])
         return DataFrame(schema=self._schema, rows=self._rows[offset : offset + length])
 
+    def filter(self, mask):
+        """
+        Select rows from the DataFRame. The DataFrame is filtered based on boolean array.
+        """
+        return DataFrame(schema=self._schema, rows=(t for t, m in zip(self._rows, mask) if m))
+
     def row(self, i):
         self.materialize()
         return self._rows[i]
 
     def fetchone(self):
         try:
             return next(self._cursor)
```

### Comparing `orso-0.0.8/orso/display.py` & `orso-0.0.9/orso/display.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.8/orso/exceptions.py` & `orso-0.0.9/orso/exceptions.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.8/orso/row.py` & `orso-0.0.9/orso/row.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.8/orso/version.py` & `orso-0.0.9/orso/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.8"
-__author__ = "@joocer"
+__version__: str = "0.0.9"
+__author__: str = "@joocer"
```

### Comparing `orso-0.0.8/orso.egg-info/PKG-INFO` & `orso-0.0.9/orso.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orso
-Version: 0.0.8
+Version: 0.0.9
 Summary: 🐻 Dataframe Library
 Home-page: https://github.com/mabel-dev/orso/
 Author: @joocer
 Author-email: justin.joyce@joocer.com
 Maintainer: @joocer
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,15 +22,17 @@
 
 </div>
 
 Orso is not intended to compete with [Polars](https://www.pola.rs/) or [Pandas](https://pandas.pydata.org/) (or your favorite DataFrame technology), instead it is developed as a common layer for HadroDB and Opteryx.
 
 ## License
 
-[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mabel-dev/orso/blob/main/LICENSE)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mabel-dev/orso/blob/master/LICENSE)
+
+Orso is licensed under Apache 2.0 unless explicitly indicated otherwise.
 
 ## Status
 
 [![Status](https://img.shields.io/badge/Status-alpha-orange)](https://github.com/mabel-dev/orso)
 
 Orso is in alpha. Alpha means different things to different people, to us, being alpha means:
```

### Comparing `orso-0.0.8/setup.py` & `orso-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.8/tests/test_converters_arrow.py` & `orso-0.0.9/tests/test_converters_arrow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import sys
 
-import pandas
 import pyarrow
 
 sys.path.insert(1, os.path.join(sys.path[0], ".."))
 
 from orso import converters
```

### Comparing `orso-0.0.8/tests/test_dataframe.py` & `orso-0.0.9/tests/test_dataframe.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 
 sys.path.insert(1, os.path.join(sys.path[0], ".."))
 
 from orso.dataframe import DataFrame
 from orso.row import Row
 
 
-@pytest.fixture
-def schema():
+def create_schema():
     return {
         "A": {"type": int, "nullable": False},
         "B": {"type": str, "nullable": True},
         "C": {"type": float, "nullable": False},
     }
 
 
-@pytest.fixture
-def rows():
+def create_rows():
     row_factory = Row.create_class(
         {
             "A": {"type": int, "nullable": False},
             "B": {"type": str, "nullable": True},
             "C": {"type": float, "nullable": False},
         }
     )
@@ -32,39 +30,45 @@
         row_factory([2, "b", 2.2]),
         row_factory([3, "c", 3.3]),
         row_factory([4, None, 4.4]),
         row_factory([5, "e", 5.5]),
     )
 
 
-@pytest.fixture
-def dataframe(schema, rows):
+def create_dataframe():
+    schema = create_schema()
+    rows = create_rows()
     return DataFrame(rows=rows, schema=schema)
 
 
-def test_dataframe_materialize(dataframe):
+def test_dataframe_materialize():
+    dataframe = create_dataframe()
     dataframe.materialize()
     assert isinstance(dataframe._rows, list)
 
 
-def test_dataframe_collect(dataframe):
+def test_dataframe_collect():
+    dataframe = create_dataframe()
     result = dataframe.collect(["A", "C"])
     assert result == ([1, 2, 3, 4, 5], [1.1, 2.2, 3.3, 4.4, 5.5])
 
 
-def test_dataframe_slice(dataframe):
+def test_dataframe_slice():
+    dataframe = create_dataframe()
     result = dataframe.slice(offset=1, length=2)
     assert len(result) == 2
 
 
-def test_dataframe_iter(dataframe):
+def test_dataframe_iter():
+    dataframe = create_dataframe()
     assert len(list(dataframe)) == 5
 
 
-def test_dataframe_len(dataframe):
+def test_dataframe_len():
+    dataframe = create_dataframe()
     assert len(dataframe) == 5
 
 
 def test_dataframe_user_init():
     # fmt:off
     cities = [
         {"name": "Tokyo", "population": 13929286, "country": "Japan", "founded": "1457", "area": 2191, "language": "Japanese"},
@@ -73,7 +77,28 @@
         {"name": "Mumbai", "population": 18500000, "country": "India", "founded": "7th century BC", "area": 603.4, "language": "Hindi, English"},
         {"name": "Cape Town", "population": 433688, "country": "South Africa", "founded": "1652", "area": 400, "language": "Afrikaans, English"},
     ]
     # fmt:on
     df = DataFrame(cities)
     assert df.column_names == ("name", "population", "country", "founded", "area", "language")
     assert df.rowcount == 5
+
+
+def test_dataframe_filter():
+    # Filter rows where column A is greater than 2
+    dataframe = create_dataframe()
+    mask = [row[0] > 2 for row in dataframe]
+    filtered_dataframe = dataframe.filter(mask)
+    assert len(filtered_dataframe) == 3
+    assert filtered_dataframe.collect(["A"]) == ([3, 4, 5],)
+
+
+if __name__ == "__main__":  # prgama: nocover
+    test_dataframe_materialize()
+    test_dataframe_collect()
+    test_dataframe_slice()
+    test_dataframe_iter()
+    test_dataframe_len()
+    test_dataframe_user_init()
+    test_dataframe_filter()
+
+    print("✅ okay")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `orso-0.0.8/tests/test_fetching.py` & `orso-0.0.9/tests/test_fetching.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.8/tests/test_load_from_pyarrow.py` & `orso-0.0.9/tests/test_load_from_pyarrow.py`

 * *Files identical despite different names*

