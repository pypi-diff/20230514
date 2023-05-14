# Comparing `tmp/Zeraora-0.2.8.tar.gz` & `tmp/Zeraora-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.8.tar", last modified: Thu May 11 07:36:58 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.9.tar", last modified: Sun May 14 17:06:30 2023, max compression
```

## Comparing `Zeraora-0.2.8.tar` & `Zeraora-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:36:58.000000 Zeraora-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-11 07:36:58.000000 Zeraora-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-11 07:36:39.000000 Zeraora-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:36:58.000000 Zeraora-0.2.8/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-11 07:36:57.000000 Zeraora-0.2.8/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 07:36:57.000000 Zeraora-0.2.8/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:36:57.000000 Zeraora-0.2.8/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 07:36:57.000000 Zeraora-0.2.8/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:36:58.000000 Zeraora-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-11 07:36:39.000000 Zeraora-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:36:58.000000 Zeraora-0.2.8/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/divisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:36:58.000000 Zeraora-0.2.8/zeraora/djangobase/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/djangobase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/djangobase/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/typeclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:06:30.000000 Zeraora-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-14 17:06:30.000000 Zeraora-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-14 17:06:17.000000 Zeraora-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:06:30.000000 Zeraora-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-14 17:06:17.000000 Zeraora-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:06:30.000000 Zeraora-0.2.9/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/divisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:06:30.000000 Zeraora-0.2.9/zeraora/djangobase/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/djangobase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/djangobase/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/typeclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/utils.py
```

### Comparing `Zeraora-0.2.8/PKG-INFO` & `Zeraora-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.8
+Version: 0.2.9
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.2.8 Summary:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.2.9 Summary:
 ä¸ä¸ªåå«ååå·¥å·ç±»åå¿«æ·å½æ°çå·¥å·åºãA original utility
 Python package. Home-page: https://github.com/aixcyi/zeraora Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com License: MIT Project-
 URL: Source, https://github.com/aixcyi/zeraora Project-URL: Tracker, https://
 github.com/aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
                 [https://img.shields.io/badge/Python-3.7%20%2B-
```

### Comparing `Zeraora-0.2.8/README.md` & `Zeraora-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.8/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.9/Zeraora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.8
+Version: 0.2.9
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.2.8 Summary:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.2.9 Summary:
 ä¸ä¸ªåå«ååå·¥å·ç±»åå¿«æ·å½æ°çå·¥å·åºãA original utility
 Python package. Home-page: https://github.com/aixcyi/zeraora Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com License: MIT Project-
 URL: Source, https://github.com/aixcyi/zeraora Project-URL: Tracker, https://
 github.com/aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
                 [https://img.shields.io/badge/Python-3.7%20%2B-
```

### Comparing `Zeraora-0.2.8/setup.py` & `Zeraora-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.8/zeraora/__init__.py` & `Zeraora-0.2.9/zeraora/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 )
 from .utils import (
     BearTimer,
     ReprMixin,
 )
 
 __author__ = 'aixcyi'
-__version__ = (0, 2, 8)
-version = '0.2.8'
+__version__ = (0, 2, 9)
+version = '0.2.9'
 
 # Django makemigrations 会在 CreateModel 里插入参数
 # bases=(zeraora.utils.ReprMixin, models.Model)
 # 导致对 zeraora 产生依赖，这里改变 ReprMixin 所在包地址，
 # 尽量减少因为改变内部包结构导致对外部的影响。
 ReprMixin.__module__ = 'zeraora'
```

### Comparing `Zeraora-0.2.8/zeraora/charsets.py` & `Zeraora-0.2.9/zeraora/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.8/zeraora/checkers.py` & `Zeraora-0.2.9/zeraora/checkers.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.8/zeraora/converters.py` & `Zeraora-0.2.9/zeraora/converters.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.8/zeraora/divisions.py` & `Zeraora-0.2.9/zeraora/divisions.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.8/zeraora/djangobase/mixins.py` & `Zeraora-0.2.9/zeraora/djangobase/mixins.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.8/zeraora/generators.py` & `Zeraora-0.2.9/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.8/zeraora/typeclasses.py` & `Zeraora-0.2.9/zeraora/typeclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,52 +274,15 @@
     """用于创建值是字符串的带有标签文本的枚举。"""
 
     def _generate_next_value_(name, start, count, last_values):
         return name
 
 
 class ItemsMeta(enum.EnumMeta):
-    """
-    用于创建带有任意属性的枚举的类（元类）。
-
-    >>> from enum import Enum
-    >>>
-    >>> class YearInSchool(Enum, metaclass=ItemsMeta):
-    >>>     FRESHMAN = 1, 'FR', 0xE35314, 'Freshman'
-    >>>     SOPHOMORE = 2, 'SO', 0xED15B4, 'Sophomore'
-    >>>     JUNIOR = 3, 'JR', 0x9B3CED, 'Junior'
-    >>>     SENIOR = 4, 'SR', 0xA0408E, 'Senior'
-    >>>     GRADUATE = 5, 'GR', 0x518CCC, 'Graduate'
-    >>>
-    >>>     __properties__ = 'code', 'color', 'label'
-    >>>
-    >>>     @property
-    >>>     def code(self) -> str:
-    >>>         return self._code_
-    >>>
-    >>>     @property
-    >>>     def color(self) -> int:
-    >>>         return self._color_
-    >>>
-    >>>     @property
-    >>>     def label(self) -> str:
-    >>>         return self._label_
-    >>>
-    >>> print(YearInSchool.SENIOR.name)  # 'SENIOR'
-    >>> print(YearInSchool.SENIOR.value)  # 4
-    >>> print(YearInSchool.SENIOR.code)  # 'SR'
-    >>> print(hex(YearInSchool.SENIOR.color))  # '0xa0408e'
-    >>> print(YearInSchool.SENIOR.label)  # 'Senior'
-    >>>
-    >>> print(YearInSchool.names)  # ['FRESHMAN', 'SOPHOMORE', ...]
-    >>> print(YearInSchool.values)  # [1, 2, 3, 4, 5]
-    >>> print(YearInSchool.codes)  # ['FR', 'SO', 'JR', 'SR', 'GR']
-    >>> print(YearInSchool.colors)  # [14897940, 15537588, ...]
-    >>> print(YearInSchool.labels)  # ['Freshman', 'Sophomore', ...]
-    """
+    """用于创建带有任意属性的枚举的类（元类）。"""
 
     def __new__(metacls, classname, bases, classdict, **kwds):
         # 获取属性名（pks）
         if '__properties__' not in classdict:
             raise AttributeError(
                 f'{classname} 使用了 {metacls.__name__}，'
                 f'因此必须定义一个名为 __properties__ 的属性。'
@@ -363,15 +326,15 @@
     def __getattr__(cls, name):
         if not isinstance(name, str):
             raise TypeError
         if name[:-1] in cls.__properties__ and name.endswith('s'):
             return [getattr(member, name[:-1]) for member in cls]
         if name[:-2] in cls.__properties__ and name.endswith('es'):
             return [getattr(member, name[:-2]) for member in cls]
-        return cls.__getattribute__(cls, name)
+        return object.__getattribute__(cls, name)
 
     @property
     def names(cls):
         empty = ["__empty__"] if hasattr(cls, "__empty__") else []
         return empty + [member.name for member in cls]
 
     @property
@@ -384,13 +347,48 @@
         empty = [(None, cls.__empty__)] if hasattr(cls, "__empty__") else []
         return empty + [(member.value, member.label) for member in cls]
 
 
 class Items(enum.Enum, metaclass=ItemsMeta):
     """
     用于创建带有任意属性的枚举。
+
+    >>> from enum import Enum
+    >>>
+    >>> class YearInSchool(Items):
+    >>>     FRESHMAN = 1, 'FR', 0xE35314, 'Freshman'
+    >>>     SOPHOMORE = 2, 'SO', 0xED15B4, 'Sophomore'
+    >>>     JUNIOR = 3, 'JR', 0x9B3CED, 'Junior'
+    >>>     SENIOR = 4, 'SR', 0xA0408E, 'Senior'
+    >>>     GRADUATE = 5, 'GR', 0x518CCC, 'Graduate'
+    >>>
+    >>>     __properties__ = 'code', 'color', 'label'
+    >>>
+    >>>     @property
+    >>>     def code(self) -> str:
+    >>>         return self._code_
+    >>>
+    >>>     @property
+    >>>     def color(self) -> int:
+    >>>         return self._color_
+    >>>
+    >>>     @property
+    >>>     def label(self) -> str:
+    >>>         return self._label_
+    >>>
+    >>> print(YearInSchool.SENIOR.name)  # 'SENIOR'
+    >>> print(YearInSchool.SENIOR.value)  # 4
+    >>> print(YearInSchool.SENIOR.code)  # 'SR'
+    >>> print(hex(YearInSchool.SENIOR.color))  # '0xa0408e'
+    >>> print(YearInSchool.SENIOR.label)  # 'Senior'
+    >>>
+    >>> print(YearInSchool.names)  # ['FRESHMAN', 'SOPHOMORE', ...]
+    >>> print(YearInSchool.values)  # [1, 2, 3, 4, 5]
+    >>> print(YearInSchool.codes)  # ['FR', 'SO', 'JR', 'SR', 'GR']
+    >>> print(YearInSchool.colors)  # [14897940, 15537588, ...]
+    >>> print(YearInSchool.labels)  # ['Freshman', 'Sophomore', ...]
     """
     __properties__ = ()
 
     def __repr__(self):
         # 枚举也算一种常量，直接按路径查找即可，故舍去附加的属性
         return f"{self.__class__.__qualname__}.{self._name_}"
```

### Comparing `Zeraora-0.2.8/zeraora/utils.py` & `Zeraora-0.2.9/zeraora/utils.py`

 * *Files identical despite different names*

