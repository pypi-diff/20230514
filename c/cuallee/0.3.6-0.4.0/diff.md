# Comparing `tmp/cuallee-0.3.6.tar.gz` & `tmp/cuallee-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuallee-0.3.6.tar", last modified: Mon Feb 20 22:59:35 2023, max compression
+gzip compressed data, was "cuallee-0.4.0.tar", last modified: Sun May 14 14:52:22 2023, max compression
```

## Comparing `cuallee-0.3.6.tar` & `cuallee-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-02-20 22:59:35.904522 cuallee-0.3.6/
--rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.3.6/LICENSE
--rw-r--r--   0 herminio  (1000) herminio  (1000)    13569 2023-02-20 22:59:35.904522 cuallee-0.3.6/PKG-INFO
--rw-rw-r--   0 herminio  (1000) herminio  (1000)    12776 2022-12-04 15:22:23.000000 cuallee-0.3.6/README.md
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-02-20 22:59:35.904522 cuallee-0.3.6/cuallee/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    20273 2022-12-10 01:22:36.000000 cuallee-0.3.6/cuallee/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     9797 2022-12-04 15:12:29.000000 cuallee-0.3.6/cuallee/duckdb_validation.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-02-20 22:59:35.904522 cuallee-0.3.6/cuallee/iso/
--rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2022-12-10 00:22:19.000000 cuallee-0.3.6/cuallee/iso/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     1457 2023-02-20 18:36:38.000000 cuallee-0.3.6/cuallee/iso/checks.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    12996 2022-12-04 15:12:29.000000 cuallee-0.3.6/cuallee/pandas_validation.py
--rw-rw-r--   0 herminio  (1000) herminio  (1000)        0 2022-11-26 21:58:56.000000 cuallee-0.3.6/cuallee/polars.validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    30990 2023-02-20 22:43:29.000000 cuallee-0.3.6/cuallee/pyspark_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2022-12-04 15:12:29.000000 cuallee-0.3.6/cuallee/snowpark_validation.py
--rw-rw-r--   0 herminio  (1000) herminio  (1000)     2043 2022-10-23 12:45:17.000000 cuallee-0.3.6/cuallee/utils.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-02-20 22:59:35.904522 cuallee-0.3.6/cuallee.egg-info/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    13569 2023-02-20 22:59:35.000000 cuallee-0.3.6/cuallee.egg-info/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-02-20 22:59:35.000000 cuallee-0.3.6/cuallee.egg-info/SOURCES.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-02-20 22:59:35.000000 cuallee-0.3.6/cuallee.egg-info/dependency_links.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)      327 2023-02-20 22:59:35.000000 cuallee-0.3.6/cuallee.egg-info/requires.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-02-20 22:59:35.000000 cuallee-0.3.6/cuallee.egg-info/top_level.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)     1228 2023-02-20 22:59:28.000000 cuallee-0.3.6/pyproject.toml
--rw-rw-r--   0 herminio  (1000) herminio  (1000)      110 2023-02-20 22:59:35.904522 cuallee-0.3.6/setup.cfg
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-05-14 14:52:22.406522 cuallee-0.4.0/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    11357 2022-10-08 07:12:42.000000 cuallee-0.4.0/LICENSE
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    13591 2023-05-14 14:52:22.406522 cuallee-0.4.0/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    12798 2023-05-14 14:50:48.000000 cuallee-0.4.0/README.md
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-05-14 14:52:22.406522 cuallee-0.4.0/cuallee/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    20284 2023-05-14 14:49:13.000000 cuallee-0.4.0/cuallee/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     9876 2023-05-14 14:49:09.000000 cuallee-0.4.0/cuallee/duckdb_validation.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-05-14 14:52:22.406522 cuallee-0.4.0/cuallee/iso/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-05-14 14:49:13.000000 cuallee-0.4.0/cuallee/iso/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-05-14 14:49:13.000000 cuallee-0.4.0/cuallee/iso/checks.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-05-14 14:49:13.000000 cuallee-0.4.0/cuallee/pandas_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-05-14 09:02:43.000000 cuallee-0.4.0/cuallee/polars.validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    31138 2023-05-14 14:49:09.000000 cuallee-0.4.0/cuallee/pyspark_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2023-05-14 09:02:43.000000 cuallee-0.4.0/cuallee/snowpark_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     2043 2023-05-14 09:02:43.000000 cuallee-0.4.0/cuallee/utils.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-05-14 14:52:22.406522 cuallee-0.4.0/cuallee.egg-info/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    13591 2023-05-14 14:52:22.000000 cuallee-0.4.0/cuallee.egg-info/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-05-14 14:52:22.000000 cuallee-0.4.0/cuallee.egg-info/SOURCES.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-05-14 14:52:22.000000 cuallee-0.4.0/cuallee.egg-info/dependency_links.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      281 2023-05-14 14:52:22.000000 cuallee-0.4.0/cuallee.egg-info/requires.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-05-14 14:52:22.000000 cuallee-0.4.0/cuallee.egg-info/top_level.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     1164 2023-05-14 14:49:13.000000 cuallee-0.4.0/pyproject.toml
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-05-14 14:52:22.406522 cuallee-0.4.0/setup.cfg
```

### Comparing `cuallee-0.3.6/LICENSE` & `cuallee-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuallee-0.3.6/PKG-INFO` & `cuallee-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.3.6
+Version: 0.4.0
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,18 +35,18 @@
 
 ## Support
 
 `cuallee` is the data quality framework truly dataframe agnostic.
 
 Provider | API | Versions
  ------- | ----------- | ------
-![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.0.0`
-![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.3.x`, `3.2.x`
-![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")|`pandas`|`1.5.x`, `1.4.x`
-![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb`|`0.6.0`
+![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
+![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
+![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
+![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
 ![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
 [![PyPI version](https://badge.fury.io/py/cuallee.svg)](https://badge.fury.io/py/cuallee)
 [![ci](https://github.com/canimus/cuallee/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canimus/cuallee/actions/workflows/ci.yml)
```

### Comparing `cuallee-0.3.6/README.md` & `cuallee-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 ## Support
 
 `cuallee` is the data quality framework truly dataframe agnostic.
 
 Provider | API | Versions
  ------- | ----------- | ------
-![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.0.0`
-![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.3.x`, `3.2.x`
-![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")|`pandas`|`1.5.x`, `1.4.x`
-![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb`|`0.6.0`
+![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
+![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
+![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
+![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
 ![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
 [![PyPI version](https://badge.fury.io/py/cuallee.svg)](https://badge.fury.io/py/cuallee)
 [![ci](https://github.com/canimus/cuallee/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canimus/cuallee/actions/workflows/ci.yml)
```

### Comparing `cuallee-0.3.6/cuallee/__init__.py` & `cuallee-0.4.0/cuallee/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 
 
 class Check:
     def __init__(
         self,
         level: Union[CheckLevel, int],
         name: str,
+        *,
         execution_date: datetime = datetime.today(),
         table_name: str = None,
     ):
         """A container of data quality rules."""
         self._rule: Dict[str, Rule] = {}
         # TODO: Should be a compute engine protocol
         self.compute_engine: ModuleType
```

### Comparing `cuallee-0.3.6/cuallee/duckdb_validation.py` & `cuallee-0.4.0/cuallee/duckdb_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 
     def is_on_schedule(self, rule: Rule) -> str:
         return (
             f"SUM(CAST(EXTRACT(hour from {rule.column}) BETWEEN {rule.value[0]} AND {rule.value[1]} AS INTEGER))"
         )
 
     def is_daily(self, rule: Rule) -> str:
+        """Returns the number or violations and matches on a daily schedule"""
         if rule.value is None:
             day_mask = tuple([1, 2, 3, 4, 5])
         else:
             day_mask = rule.value
 
         template = Template(
             """
```

### Comparing `cuallee-0.3.6/cuallee/iso/checks.py` & `cuallee-0.4.0/cuallee/iso/checks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,65 @@
 from lxml import etree
 import requests
-from dotenv import load_dotenv
 from dataclasses import dataclass
 from typing import List
 import os
 from operator import attrgetter as at
 from functools import lru_cache
+import pandas as pd
+from toolz import first
 
 @dataclass
 class Currency:
     country_name: str
     currency_name: str
     currency: str = None
     currency_number: str = None
     currency_units: str = None
 
+@lru_cache
+def _load_currencies():
+    """ External download from ISO website of currencies in XML format """
+    DEFAULT_ENDPOINT_4217 = "https://www.six-group.com/dam/download/financial-information/data-center/iso-currrency/lists/list-one.xml"
+    response = requests.get(os.getenv("ISO_4217_ENDPOINT", DEFAULT_ENDPOINT_4217))
+    xml = etree.fromstring(response.text.encode("utf-8"))
+
+    def _get_ccy(element : etree._Element) -> Currency:
+        return at("currency")(Currency(*[tag.text for tag in element.getchildren()]))
+
+    return set(filter(None, (map(_get_ccy, xml.xpath("//CcyNtry")))))
+
+@lru_cache
+def _load_countries():
+    """ External download from Google shared data of country codes and locations """
+    DEFAULT_ENDPOINT_3166 = "https://developers.google.com/public-data/docs/canonical/countries_csv"
+    response = pd.read_html(os.getenv("ISO_3166_ENDPOINT", DEFAULT_ENDPOINT_3166))
+    return first(response)["country"].str.upper().dropna().tolist()
+
+
 class ISO():
+    """ Abstraction of checks related to ISO standards """
     CCY_CODE = "currency"
     CCY_NUMBER = "currency_number"
+    COUNTRY_CODE = "country"
+    COUNTRY_NAME = "name"
 
-    @lru_cache
-    def _load_currencies(self, by_field : str = CCY_CODE):
-        """Internal helper method to load all currencies from default environment location"""
-        load_dotenv()
-        response = requests.get(os.getenv("ISO_4217_ENDPOINT", "https://www.six-group.com/dam/download/financial-information/data-center/iso-currrency/lists/list-one.xml"))
-        xml = etree.fromstring(response.text.encode("utf-8"))
-
-        def _get_ccy(element : etree._Element) -> Currency:
-            return at(by_field)(Currency(*[tag.text for tag in element.getchildren()]))
-
-        return set(filter(None, (map(_get_ccy, xml.xpath("//CcyNtry")))))
-
-    def __init__(self, check, currency_field : str = CCY_CODE):
+    def __init__(self, check):
         self._check = check
-        self._ccy = self._load_currencies(currency_field)
+        self._ccy = []
+        self._countries = []
 
     def iso_4217(self, column : str):
         """It verifies a field against the international standard currency codes via code or number fields from ISO 4217"""
+        self._ccy = _load_currencies()
         self._check.is_in(column, self._ccy)
-    
+        return self._check
+    
+    def iso_3166(self, column: str):
+        """ Verifies that country codes are valid against the ISO standard 3166 """
+        self._countries = _load_countries()
+        self._check.is_in(column, self._countries)
+        return self._check
+    
+
+    iso_currencies = iso_4217
+    iso_countries = iso_3166
```

### Comparing `cuallee-0.3.6/cuallee/pandas_validation.py` & `cuallee-0.4.0/cuallee/pandas_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,25 +166,24 @@
 
         lower, upper = (
             dataframe.loc[:, rule.column].agg([np.min, np.max]).dt.strftime("%Y-%m-%d")
         )
         sequence = (
             pd.date_range(start=lower, end=upper, freq="D").rename("ts").to_frame()
         )
-        sequence = (
+        sequence = list(
             sequence[sequence.ts.dt.dayofweek.isin(day_mask)]
             .reset_index(drop=True)
             .ts.unique()
-            .astype(np.datetime64)
+            .astype("datetime64[ms]")
         )
 
-        delivery = (
+        delivery = list(
             dataframe[dataframe[rule.column].dt.dayofweek.isin(day_mask)][rule.column]
-            .dt.date.astype(np.datetime64)
-            .values
+            .dt.date.astype("datetime64[ms]")
         )
 
         # No difference between sequence of daily as a complex number
         return complex(len(dataframe), len(set(sequence).difference(delivery)))
 
     def is_inside_interquartile_range(
         self, rule: Rule, dataframe: pd.DataFrame
```

### Comparing `cuallee-0.3.6/cuallee/pyspark_validation.py` & `cuallee-0.4.0/cuallee/pyspark_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         return self.compute_instruction
 
     def is_unique(self, rule: Rule):
         """Validation for unique values in column"""
         predicate = None  # F.count_distinct(F.col(rule.column))
         self.compute_instruction = ComputeInstruction(
             predicate,
-            F.count_distinct(F.col(f"`{rule.column}`")),
+            F.approx_count_distinct(F.col(f"`{rule.column}`")),
             ComputeMethod.SELECT,
         )
         return self.compute_instruction
 
     def are_unique(self, rule: Rule):
         """Validation for unique values in a group of columns"""
         predicate = None  # TODO:  .groupBy("value").count.filter("count > 1")
@@ -563,34 +563,43 @@
 ) -> List[str]:
     """Internal method to search for column names based on data type"""
     return set(
         [f.name for f in dataframe.schema.fields if isinstance(f.dataType, field_type)]  # type: ignore
     )
 
 
+def _replace_observe_compute(computed_expressions: dict) -> dict:
+    """Replace observe based check with select"""
+    print(
+        "[😔]"
+        + Fore.YELLOW
+        + " PySpark < 3.3.0 | When you upgrade checks will run 2x faster."
+    )
+    print(Style.RESET_ALL)
+    select_only_expressions = {}
+    for k, v in computed_expressions.items():
+        instruction = v
+        if instruction.compute_method.name == ComputeMethod.OBSERVE.name:
+            instruction.compute_method = ComputeMethod.SELECT
+        select_only_expressions[k] = instruction
+    return select_only_expressions
+
+
 def _compute_observe_method(
     compute_set: Dict[str, ComputeInstruction], dataframe: DataFrame
 ) -> Tuple[int, Dict]:
     """Compute rules throught spark Observation"""
 
     # Filter expression directed to observe
     _observe = lambda x: x.compute_method.name == ComputeMethod.OBSERVE.name
     observe = valfilter(_observe, compute_set)
 
-    try:
+    if observe:
         from pyspark.sql import Observation
-    except:
-        print(
-            "[😔]"
-            + Fore.YELLOW
-            + " PySpark < 3.3.0 | When you upgrade checks will run 2x faster."
-        )
-        print(Style.RESET_ALL)
 
-    if observe:
         observation = Observation("observation")
 
         df_observation = dataframe.observe(
             observation,
             *[
                 compute_instruction.expression.alias(hash_key)
                 for hash_key, compute_instruction in observe.items()
@@ -726,21 +735,15 @@
     else:
         # TODO: Check should have options for compute engine
         spark = SparkSession.builder.getOrCreate()
 
     # Compute the expression
     computed_expressions = compute(check._rule)
     if int(spark.version.replace(".", "")) < 330:
-        select_only_expressions = {}
-        for k, v in computed_expressions.items():
-            instruction = v
-            if instruction.compute_method == "observe":
-                instruction.compute_method = "select"
-            select_only_expressions[k] = instruction
-        computed_expressions = select_only_expressions
+        computed_expressions = _replace_observe_compute(computed_expressions)
 
     rows, observation_result = _compute_observe_method(computed_expressions, dataframe)
     select_result = _compute_select_method(computed_expressions, dataframe)
     transform_result = _compute_transform_method(computed_expressions, dataframe)
 
     unified_results = {**observation_result, **select_result, **transform_result}
     logger.debug(unified_results)
```

### Comparing `cuallee-0.3.6/cuallee/snowpark_validation.py` & `cuallee-0.4.0/cuallee/snowpark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.3.6/cuallee/utils.py` & `cuallee-0.4.0/cuallee/utils.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.3.6/cuallee.egg-info/PKG-INFO` & `cuallee-0.4.0/cuallee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.3.6
+Version: 0.4.0
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,18 +35,18 @@
 
 ## Support
 
 `cuallee` is the data quality framework truly dataframe agnostic.
 
 Provider | API | Versions
  ------- | ----------- | ------
-![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.0.0`
-![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.3.x`, `3.2.x`
-![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")|`pandas`|`1.5.x`, `1.4.x`
-![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb`|`0.6.0`
+![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
+![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
+![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
+![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
 ![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
 [![PyPI version](https://badge.fury.io/py/cuallee.svg)](https://badge.fury.io/py/cuallee)
 [![ci](https://github.com/canimus/cuallee/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canimus/cuallee/actions/workflows/ci.yml)
```

### Comparing `cuallee-0.3.6/pyproject.toml` & `cuallee-0.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cuallee"
-version = "0.3.6"
+version = "0.4.0"
 authors = [
   { name="Virginie Grosboillot", email="vestalisvirginis@gmail.com" },
   { name="Herminio Vazquez", email="canimus@gmail.com"}
 ]
 description = "Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -16,38 +16,36 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "colorama >= 0.4.6",
     "toolz >= 0.12.0",
-    "pygments >= 2.13.0",
-    "lxml >= 4.9.1",
-    "requests >= 2.28.2",
-    "python-dotenv >= 0.21.0"
+    "pygments >= 2.15.1",
+    "lxml >= 4.9.2"
 ]
 
 [project.optional-dependencies]
 pyspark = [
-  "pyspark>=3.0.1"
+  "pyspark>=3.4.0"
 ]
 snowpark = [
-  "snowflake-snowpark-python>=0.0.12"
+  "snowflake-snowpark-python>=1.4.0",
+  "pyarrow >= 10.0.1"
 ]
 pandas = [
-  "pandas>=1.4.1"
+  "pandas>=2.0.1"
 ]
 duckdb = [
-  "duckdb>=0.6.0"
+  "duckdb>=0.7.1"
 ]
 polars = [
   "polars>=0.14.29"
 ]
 iso = [
-  "python-dotenv >= 0.21.0",
   "lxml >= 4.9.1"
 ]
 test = [
   "pytest",
   "pytest-cov",
   "pendulum >= 2.1.2"
 ]
```

