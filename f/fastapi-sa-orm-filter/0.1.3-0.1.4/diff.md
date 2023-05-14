# Comparing `tmp/fastapi-sa-orm-filter-0.1.3.tar.gz` & `tmp/fastapi-sa-orm-filter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sa-orm-filter-0.1.3.tar", last modified: Thu May 11 06:49:19 2023, max compression
+gzip compressed data, was "fastapi-sa-orm-filter-0.1.4.tar", last modified: Sun May 14 11:37:12 2023, max compression
```

## Comparing `fastapi-sa-orm-filter-0.1.3.tar` & `fastapi-sa-orm-filter-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.3/.github/workflows/ci_filter.yml
--rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.3/LICENSE
--rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.3/Pipfile
--rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.3/Pipfile.lock
--rw-r--r--   0        0        0     2529 2023-05-11 06:46:05.227485 fastapi-sa-orm-filter-0.1.3/README.md
--rw-r--r--   0        0        0      111 2023-05-11 06:49:13.039045 fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/__init__.py
--rw-r--r--   0        0        0     6617 2023-05-11 06:36:12.456633 fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/main.py
--rw-r--r--   0        0        0      497 2023-05-10 20:18:36.372884 fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/operators.py
--rw-r--r--   0        0        0     4936 2023-05-11 06:30:01.548954 fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/parsers.py
--rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.3/pytest.ini
--rw-r--r--   0        0        0     3364 2023-05-09 20:41:44.249744 fastapi-sa-orm-filter-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0    17207 2023-05-11 06:40:39.744176 fastapi-sa-orm-filter-0.1.3/tests/test_filter.py
--rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.3/tests/utils.py
--rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.4/.github/workflows/ci_filter.yml
+-rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.4/LICENSE
+-rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.4/Pipfile
+-rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.4/Pipfile.lock
+-rw-r--r--   0        0        0     3335 2023-05-14 11:36:07.168548 fastapi-sa-orm-filter-0.1.4/README.md
+-rw-r--r--   0        0        0      111 2023-05-14 11:37:04.453163 fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/__init__.py
+-rw-r--r--   0        0        0     6820 2023-05-14 11:36:07.164548 fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/main.py
+-rw-r--r--   0        0        0      497 2023-05-10 20:18:36.372884 fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/operators.py
+-rw-r--r--   0        0        0     4945 2023-05-14 07:33:57.502154 fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/parsers.py
+-rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.4/pytest.ini
+-rw-r--r--   0        0        0     4059 2023-05-14 11:36:38.456872 fastapi-sa-orm-filter-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0    19083 2023-05-14 11:20:17.304458 fastapi-sa-orm-filter-0.1.4/tests/test_filter.py
+-rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.4/tests/utils.py
+-rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.4/PKG-INFO
```

### Comparing `fastapi-sa-orm-filter-0.1.3/.github/workflows/ci_filter.yml` & `fastapi-sa-orm-filter-0.1.4/.github/workflows/ci_filter.yml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.3/LICENSE` & `fastapi-sa-orm-filter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.3/Pipfile.lock` & `fastapi-sa-orm-filter-0.1.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.3/README.md` & `fastapi-sa-orm-filter-0.1.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -71,14 +71,38 @@
 ### Supported query string format
 
 * field_name__eq=value
 * field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2&order_by=-field_name
 
+### Modify query for custom selection
+```shell
+# Create a class inherited from FilterCore and rewrite 'construct_query' method.
+# Original method is:
+def get_unordered_query(self, conditions):
+    unordered_query = select(self._model).filter(or_(*conditions))
+    return unordered_query
+    
+# Rewrite example:
+class CustomFilter(FilterCore):
+    def __init__(self, model, allowed_filters):
+        super().__init__(model, allowed_filters)
+
+    def get_unordered_query(self, conditions):
+        unordered_query = select(
+            self._model.field_name1,
+            self._model.field_name2,
+            func.sum(self._model.field_name3).label("field_name3"),
+            self._model.field_name4
+        ).filter(or_(*conditions)).group_by(self._model.field_name2)
+        return unordered_query
+
+```
+
 ### Supported SQLAlchemy datatypes:
 * DATETIME
 * DATE
 * INTEGER
 * FLOAT
 * TEXT
 * VARCHAR
```

### Comparing `fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/main.py` & `fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,38 +61,41 @@
                         ),
                         model.category == 'Medicine'
                     ).order_by(model.id.desc())
         """
         split_query = self.split_by_order_by(custom_filter)
         if len(split_query) == 1:
             filter_query = self._get_filter_query(split_query[0])
-            return filter_query
+            complete_query = self.get_unordered_query(filter_query)
+            return complete_query
         filter_query_str, order_by_query_str = split_query
         filter_query = self._get_filter_query(filter_query_str)
         order_by_query = _OrderByQueryParser(self._model).get_order_by_query(order_by_query_str)
-        query = filter_query.order_by(*order_by_query)
-        return query
+        complete_query = self.get_unordered_query(filter_query).order_by(*order_by_query)
+        return complete_query
+
+    def get_unordered_query(self, conditions):
+        unordered_query = select(self._model).filter(or_(*conditions))
+        return unordered_query
 
     def _get_filter_query(self, custom_filter):
-        if not custom_filter:
-            query = select(self._model)
-            return query
-        conditions = []
+        filter_conditions = []
+        if custom_filter == '':
+            return filter_conditions
         query_parser = _FilterQueryParser(custom_filter, self._model, self._allowed_filters)
         for and_expressions in query_parser.get_parsed_query():
             and_condition = []
             for expression in and_expressions:
                 column, operator, value = expression
                 serialized_dict = self._format_expression(column, operator, value)
                 value = serialized_dict[column.name]
                 param = self._get_orm_for_field(column, operator, value)
                 and_condition.append(param)
-            conditions.append(and_(*and_condition))
-        query = select(self._model).filter(or_(*conditions))
-        return query
+            filter_conditions.append(and_(*and_condition))
+        return filter_conditions
 
     def _create_pydantic_serializer(self) -> Dict[str, ModelMetaclass]:
         """
         Create two pydantic models (optional and list field types)
         for value: str serialization
 
         :return: {
```

### Comparing `fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/parsers.py` & `fastapi-sa-orm-filter-0.1.4/fastapi_sa_orm_filter/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 
 class _FilterQueryParser:
     """
     Class parse filter part of request query string.
     """
 
     def __init__(self, query: str, model: Type[DeclarativeMeta], allowed_filters: Dict[str, List[ops]]) -> None:
-        self.query = query
-        self.model = model
-        self.allowed_filters = allowed_filters
+        self._query = query
+        self._model = model
+        self._allowed_filters = allowed_filters
 
     def get_parsed_query(self) -> List[List[Any]]:
         """
         :return:
             [
                 [[column, operator, value], [column, operator, value]],
                 [[column, operator, value]]
@@ -84,15 +84,15 @@
         to divide query string to field's conditions
 
         :return: [
                     ['field_name__operator=value', 'field_name__operator=value'],
                     ['field_name__operator=value']
                 ]
         """
-        and_blocks = [block.split("&") for block in self.query.split("|")]
+        and_blocks = [block.split("&") for block in self._query.split("|")]
         return and_blocks
 
     def _parse_expression(
         self, expression: str
     ) -> Union[Tuple[InstrumentedAttribute, str, str], HTTPException]:
         try:
             field_name, condition = expression.split("__")
@@ -100,34 +100,34 @@
         except Exception:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail="Incorrect filter request syntax,"
                 " please use pattern :"
                 "'{field_name}__{condition}={value}{conjunction}'",
             )
-        if not hasattr(self.model, field_name):
+        if not hasattr(self._model, field_name):
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail=f"DB model {self.model} doesn't have field '{field_name}'",
+                detail=f"DB model {self._model} doesn't have field '{field_name}'",
             )
         else:
-            column = getattr(self.model, field_name)
+            column = getattr(self._model, field_name)
         return column, operator, value
 
     def _validate_query_params(
         self, field_name: str, operator: str
     ) -> Optional[HTTPException]:
         """
         Check expression on valid and allowed field_name and operator
         """
-        if field_name not in self.allowed_filters:
+        if field_name not in self._allowed_filters:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail=f"Forbidden filter field '{field_name}'",
             )
-        for allow_filter in self.allowed_filters[field_name]:
+        for allow_filter in self._allowed_filters[field_name]:
             if operator == allow_filter.name:
                 return
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=f"Forbidden filter '{operator}' for '{field_name}'",
         )
```

### Comparing `fastapi-sa-orm-filter-0.1.3/pyproject.toml` & `fastapi-sa-orm-filter-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.3/tests/conftest.py` & `fastapi-sa-orm-filter-0.1.4/tests/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from datetime import date, datetime
 
 import pytest
 import pytest_asyncio
-from sqlalchemy import Column, Integer, Date, Text, String, Boolean, DateTime, Enum, Float
+from sqlalchemy import Column, Integer, Date, Text, String, Boolean, DateTime, Enum, Float, select, or_, func
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
 from sqlalchemy.orm import sessionmaker, declarative_base
 
 from fastapi_sa_orm_filter.main import FilterCore
 from fastapi_sa_orm_filter.operators import Operators as ops
 from tests.utils import JobCategory
 
@@ -79,15 +79,16 @@
         vacancy = Vacancy(
             title=f"title{i}",
             description=f"description{i}",
             salary_from=50 + i * 10,
             salary_up_to=100.725 + i * 10,
             created_at=date(2023, 5, i),
             updated_at=datetime(2023, i, 5, 15, 15, 15),
-            category=JobCategory[enum_category[i - 1]]
+            category=JobCategory[enum_category[i - 1]],
+            is_active=bool(i % 2)
         )
         vacancy_instances.append(vacancy)
     session.add_all(vacancy_instances)
     await session.commit()
 
 
 @pytest.fixture
@@ -103,7 +104,26 @@
         'is_active': [ops.eq]
     }
 
 
 @pytest.fixture
 def get_filter(get_custom_restriction):
     return FilterCore(Vacancy, get_custom_restriction)
+
+
+@pytest.fixture
+def get_custom_filter(get_custom_restriction):
+
+    class CustomFilter(FilterCore):
+        def __init__(self, model, allowed_filters):
+            super().__init__(model, allowed_filters)
+
+        def get_unordered_query(self, conditions):
+            unordered_query = select(
+                self._model.id,
+                self._model.is_active,
+                func.sum(self._model.salary_from).label("salary_from"),
+                self._model.category
+            ).filter(or_(*conditions)).group_by(self._model.is_active)
+            return unordered_query
+
+    return CustomFilter(Vacancy, get_custom_restriction)
```

### Comparing `fastapi-sa-orm-filter-0.1.3/tests/test_filter.py` & `fastapi-sa-orm-filter-0.1.4/tests/test_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,35 @@
 PydanticVacancy = sqlalchemy_to_pydantic(Vacancy)
 
 
 class ListPydanticVacancy(BaseModel):
     vacancies: List[PydanticVacancy] = []
 
 
+async def test_empty_query(session, get_filter, create_vacancies):
+    query = get_filter.get_query("")
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 10
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
+    del check_data["created_at"]
+    del check_data["updated_at"]
+    assert check_data == {
+        'id': 1,
+        'title': 'title1',
+        'description': 'description1',
+        'is_active': True,
+        'salary_from': 60,
+        'salary_up_to': 110.725,
+        'category': JobCategory.finance
+    }
+
+
 async def test_eq_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__eq=60")
     res = await session.execute(query)
     data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
     assert len(data['vacancies']) == 1
     assert isinstance(data['vacancies'][0]["created_at"], date)
     assert isinstance(data['vacancies'][0]["updated_at"], datetime)
@@ -48,15 +69,15 @@
     check_data = data['vacancies'][0].copy()
     del check_data["created_at"]
     del check_data["updated_at"]
     assert check_data == {
         'id': 2,
         'title': 'title2',
         'description': 'description2',
-        'is_active': True,
+        'is_active': False,
         'salary_from': 70,
         'salary_up_to': 120.725,
         'category': JobCategory.marketing
     }
 
 
 async def test_in_with_str(session, get_filter, create_vacancies):
@@ -90,15 +111,15 @@
     check_data = data['vacancies'][-1].copy()
     del check_data['created_at']
     del check_data['updated_at']
     assert check_data == {
         'id': 10,
         'title': 'title10',
         'description': 'description10',
-        'is_active': True,
+        'is_active': False,
         'salary_from': 150,
         'salary_up_to': 200.725,
         'category': JobCategory.miscellaneous
     }
 
 
 async def test_endswith_with_str(session, get_filter, create_vacancies):
@@ -174,26 +195,26 @@
     check_data = data['vacancies'][0].copy()
     del check_data['created_at']
     del check_data['updated_at']
     assert check_data == {
         'id': 2,
         'title': 'title2',
         'description': 'description2',
-        'is_active': True,
+        'is_active': False,
         'salary_from': 70,
         'salary_up_to': 120.725,
         'category': JobCategory.marketing
     }
 
 
 async def test_eq_with_bool(session, get_filter, create_vacancies):
     query = get_filter.get_query("is_active__eq=true")
     res = await session.execute(query)
     data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
-    assert len(data['vacancies']) == 10
+    assert len(data['vacancies']) == 5
     assert isinstance(data['vacancies'][0]["created_at"], date)
     assert isinstance(data['vacancies'][0]["updated_at"], datetime)
     check_data = data['vacancies'][0].copy()
     del check_data['created_at']
     del check_data['updated_at']
     assert check_data == {
         'id': 1,
@@ -237,15 +258,15 @@
     check_data = data['vacancies'][-1].copy()
     del check_data['created_at']
     del check_data['updated_at']
     assert check_data == {
         'id': 4,
         'title': 'title4',
         'description': 'description4',
-        'is_active': True,
+        'is_active': False,
         'salary_from': 90,
         'salary_up_to': 140.725,
         'category': JobCategory.it
     }
 
 
 async def test_between_with_date(session, get_filter, create_vacancies):
@@ -279,15 +300,15 @@
     check_data = data['vacancies'][0].copy()
     del check_data['created_at']
     del check_data['updated_at']
     assert check_data == {
         'id': 6,
         'title': 'title6',
         'description': 'description6',
-        'is_active': True,
+        'is_active': False,
         'salary_from': 110,
         'salary_up_to': 160.725,
         'category': JobCategory.medicine
     }
 
 
 async def test_enum_with_str(session, get_filter, create_vacancies):
@@ -300,15 +321,15 @@
     check_data = data['vacancies'][0].copy()
     del check_data['created_at']
     del check_data['updated_at']
     assert check_data == {
         'id': 6,
         'title': 'title6',
         'description': 'description6',
-        'is_active': True,
+        'is_active': False,
         'salary_from': 110,
         'salary_up_to': 160.725,
         'category': JobCategory.medicine
     }
 
 
 async def test_complex_query(session, get_filter, create_vacancies):
@@ -351,15 +372,15 @@
     check_data = data['vacancies'][0].copy()
     del check_data['created_at']
     del check_data['updated_at']
     assert check_data == {
         'id': 10,
         'title': 'title10',
         'description': 'description10',
-        'is_active': True,
+        'is_active': False,
         'salary_from': 150,
         'salary_up_to': 200.725,
         'category': JobCategory.miscellaneous
     }
 
 
 async def test_order_by_id(session, get_filter, create_vacancies):
@@ -372,21 +393,54 @@
     check_data = data['vacancies'][0].copy()
     del check_data["created_at"]
     del check_data["updated_at"]
     assert check_data == {
         'id': 10,
         'title': 'title10',
         'description': 'description10',
-        'is_active': True,
+        'is_active': False,
         'salary_from': 150,
         'salary_up_to': 200.725,
         'category': JobCategory.miscellaneous
     }
 
 
+async def test_custom_query(session, get_custom_filter, create_vacancies):
+    query = get_custom_filter.get_query("")
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.all()).dict(exclude_none=True)
+    assert len(data['vacancies']) == 2
+    check_data = data['vacancies'][0].copy()
+    assert check_data == {
+        'id': 2,
+        'is_active': False,
+        'salary_from': 550,
+        'category': JobCategory.marketing
+    }
+
+
+async def test_custom_complex_query(session, get_custom_filter, create_vacancies):
+    query = get_custom_filter.get_query(
+        "created_at__between=2023-05-01,2023-05-05&"
+        "updated_at__in_=2023-01-05 15:15:15,2023-05-05 15:15:15|"
+        "salary_from__gt=100&"
+        "order_by=-salary_from"
+    )
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.all()).dict(exclude_none=True)
+    assert len(data['vacancies']) == 2
+    check_data = data['vacancies'][0].copy()
+    assert check_data == {
+        'id': 6,
+        'is_active': False,
+        'salary_from': 390,
+        'category': JobCategory.medicine
+    }
+
+
 @pytest.mark.parametrize(
     "bad_filter, expected_status_code, expected_detail",
     (
         (
             "salary_from__qt=100",
             HTTP_400_BAD_REQUEST,
             "Forbidden filter 'qt' for 'salary_from'"
```

### Comparing `fastapi-sa-orm-filter-0.1.3/PKG-INFO` & `fastapi-sa-orm-filter-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sa-orm-filter
-Version: 0.1.3
+Version: 0.1.4
 Summary: FastAPI-SQLAlchemy filter, transform request query string to SQLAlchemy orm query
 Author-email: Oleksandr Zhydyk <zhydykalex@ukr.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi
 Requires-Dist: sqlalchemy
@@ -91,14 +91,38 @@
 ### Supported query string format
 
 * field_name__eq=value
 * field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2&order_by=-field_name
 
+### Modify query for custom selection
+```shell
+# Create a class inherited from FilterCore and rewrite 'construct_query' method.
+# Original method is:
+def get_unordered_query(self, conditions):
+    unordered_query = select(self._model).filter(or_(*conditions))
+    return unordered_query
+    
+# Rewrite example:
+class CustomFilter(FilterCore):
+    def __init__(self, model, allowed_filters):
+        super().__init__(model, allowed_filters)
+
+    def get_unordered_query(self, conditions):
+        unordered_query = select(
+            self._model.field_name1,
+            self._model.field_name2,
+            func.sum(self._model.field_name3).label("field_name3"),
+            self._model.field_name4
+        ).filter(or_(*conditions)).group_by(self._model.field_name2)
+        return unordered_query
+
+```
+
 ### Supported SQLAlchemy datatypes:
 * DATETIME
 * DATE
 * INTEGER
 * FLOAT
 * TEXT
 * VARCHAR
```

