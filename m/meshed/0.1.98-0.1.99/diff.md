# Comparing `tmp/meshed-0.1.98.tar.gz` & `tmp/meshed-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshed-0.1.98.tar", last modified: Tue Jan  3 13:22:58 2023, max compression
+gzip compressed data, was "meshed-0.1.99.tar", last modified: Fri Feb  3 11:55:08 2023, max compression
```

## Comparing `meshed-0.1.98.tar` & `meshed-0.1.99.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:22:58.699036 meshed-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-03 13:22:26.000000 meshed-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-01-03 13:22:58.699036 meshed-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-01-03 13:22:26.000000 meshed-0.1.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:22:58.695036 meshed-0.1.98/meshed/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    64813 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:22:58.695036 meshed-0.1.98/meshed/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/examples/online_marketing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/examples/price_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/examples/vaccine_vs_no_vaccine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:22:58.695036 meshed-0.1.98/meshed/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33997 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/ext/gk.py
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/ext/gk_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14703 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/itools.py
--rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/makers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:22:58.699036 meshed-0.1.98/meshed/scrap/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/scrap/cached_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/scrap/dask_graph_language.py
--rw-r--r--   0 runner    (1001) docker     (123)    36482 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/scrap/gk_with_networkx.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/scrap/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/scrap/wrapping_dags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:22:58.699036 meshed-0.1.98/meshed/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/objects_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_ch_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_dag_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_dag_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_dag_variadics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_itools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_makers.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/tests/utils_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27901 2023-01-03 13:22:26.000000 meshed-0.1.98/meshed/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 13:22:58.695036 meshed-0.1.98/meshed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-01-03 13:22:58.000000 meshed-0.1.98/meshed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-01-03 13:22:58.000000 meshed-0.1.98/meshed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 13:22:58.000000 meshed-0.1.98/meshed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 13:22:58.000000 meshed-0.1.98/meshed.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-01-03 13:22:58.000000 meshed-0.1.98/meshed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-03 13:22:58.000000 meshed-0.1.98/meshed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-03 13:22:58.699036 meshed-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-03 13:22:26.000000 meshed-0.1.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:55:08.461572 meshed-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-03 11:54:41.000000 meshed-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-02-03 11:55:08.461572 meshed-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-02-03 11:54:41.000000 meshed-0.1.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:55:08.457571 meshed-0.1.99/meshed/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69000 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:55:08.461572 meshed-0.1.99/meshed/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/examples/online_marketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/examples/price_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/examples/vaccine_vs_no_vaccine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:55:08.461572 meshed-0.1.99/meshed/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33997 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/ext/gk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/ext/gk_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14703 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/itools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/makers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:55:08.461572 meshed-0.1.99/meshed/scrap/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/scrap/cached_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-03 11:55:07.000000 meshed-0.1.99/meshed/scrap/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/scrap/dask_graph_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36482 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/scrap/gk_with_networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/scrap/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/scrap/wrapping_dags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-02-03 11:55:07.000000 meshed-0.1.99/meshed/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:55:08.461572 meshed-0.1.99/meshed/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/objects_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_ch_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_dag_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_dag_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_dag_variadics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_itools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_makers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-03 11:54:41.000000 meshed-0.1.99/meshed/tests/utils_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-02-03 11:55:07.000000 meshed-0.1.99/meshed/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:55:08.457571 meshed-0.1.99/meshed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-02-03 11:55:08.000000 meshed-0.1.99/meshed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-03 11:55:08.000000 meshed-0.1.99/meshed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:55:08.000000 meshed-0.1.99/meshed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:55:08.000000 meshed-0.1.99/meshed.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-03 11:55:08.000000 meshed-0.1.99/meshed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-03 11:55:08.000000 meshed-0.1.99/meshed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-03 11:55:08.461572 meshed-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-03 11:54:41.000000 meshed-0.1.99/setup.py
```

### Comparing `meshed-0.1.98/LICENSE` & `meshed-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/PKG-INFO` & `meshed-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshed
-Version: 0.1.98
+Version: 0.1.99
 Summary: Link functions up into callable objects
 Home-page: https://github.com/i2mint/meshed
 License: mit
 Description: # meshed
         
         Link functions up into callable objects (e.g. pipelines, DAGs, etc.)
```

### Comparing `meshed-0.1.98/README.md` & `meshed-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/__init__.py` & `meshed-0.1.99/meshed/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 `itools.py` contain tools that enable operations on graphs where graphs are represented
 by an adjacency Mapping.
 
 """
 
 
 from meshed.dag import DAG, ch_funcs, ch_names
-from meshed.base import FuncNode
+from meshed.base import FuncNode, compare_signatures
 from meshed.makers import code_to_dag, code_to_fnodes
 from meshed.itools import random_graph, topological_sort
 from meshed.util import (
     iterize,
     ConditionalIterize,
     instance_checker,
     replace_item_in_iterable,
```

### Comparing `meshed-0.1.98/meshed/base.py` & `meshed-0.1.99/meshed/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 """
 from collections import Counter
 from dataclasses import dataclass, field, fields
 from functools import partial, cached_property
 from typing import Callable, MutableMapping, Iterable, Union, Sized, Sequence
 
 from i2 import Sig, call_somewhat_forgivingly
-from i2.signatures import ch_variadics_to_non_variadic_kind
+from i2.signatures import (
+    ch_variadics_to_non_variadic_kind,
+    CallableComparator,
+    compare_signatures,
+)
 from meshed.util import ValidationError, NameValidationError, mk_func_name
 from meshed.itools import add_edge
 
 
 def underscore_func_node_names_maker(func: Callable, name=None, out=None):
     """This name maker will resolve names in the following fashion:
 
@@ -463,36 +467,37 @@
             f'These are not params of {type(fn).__name__}: '
             f'{params_that_are_not_init_params}'
         )
     fn_kwargs = dict(init_params, **new_attrs_values)
     return FuncNode(**fn_kwargs)
 
 
-def compare_signatures(func1, func2):
-    return Sig(func1) == Sig(func2)
-
-
 def raise_signature_mismatch_error(fn, func):
     raise ValueError(
         'You can only change the func of a FuncNode with a another func if the '
         'signatures match.\n'
         f'\t{fn=}\n'
         f'\t{Sig(fn.func)=}\n'
         f'\t{Sig(func)=}\n'
     )
 
 
+# from i2.signatures import keyed_comparator, SignatureComparator
+# if compare_func is None:
+#     compare_func = keyed_comparator(signature_comparator, key=Sig)
+
+
 def ch_func_node_func(
     fn: FuncNode,
     func: Callable,
     *,
-    compare_func=compare_signatures,
+    func_comparator: CallableComparator = compare_signatures,
     alternative=raise_signature_mismatch_error,
 ):
-    if compare_func(fn.func, func):
+    if func_comparator(fn.func, func):
         return ch_func_node_attrs(fn, func=func)
     else:
         return alternative(fn, func)
 
 
 def _keys_and_values_are_strings_validation(d: dict):
     for k, v in d.items():
```

### Comparing `meshed-0.1.98/meshed/caching.py` & `meshed-0.1.99/meshed/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Caching meshes"""
 
 from functools import cached_property
 from inspect import signature
 
-from meshed.util import func_name, Literal
+from meshed.util import func_name, LiteralVal
 
 
 def set_cached_property_attr(obj, name, value):
     cached_value = cached_property(value)
     cached_value.__set_name__(obj, name)
     setattr(obj, name, cached_value)
 
@@ -17,23 +17,23 @@
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         #         cls.__literals = []
         #         cls.__lazyprops = []
         for attr_name in (a for a in dir(cls) if not a.startswith('__')):
             attr_obj = getattr(cls, attr_name)
-            if isinstance(attr_obj, Literal):
+            if isinstance(attr_obj, LiteralVal):
                 setattr(cls, attr_name, attr_obj.val)
             #                 cls._LazyProps__literals.append(attr_name)
             else:
                 set_cached_property_attr(cls, attr_name, attr_obj)
 
     #                 cls._LazyProps__lazyprops.append(attr_name)
 
-    Literal = Literal  # just to have Literal available as LazyProps.Literal
+    Literal = LiteralVal  # just to have Literal available as LazyProps.Literal
 
 
 def add_cached_property(cls, method, attr_name=None):
     attr_name = attr_name or func_name(method)
     set_cached_property_attr(cls, attr_name, method)
     return cls
```

### Comparing `meshed-0.1.98/meshed/composition.py` & `meshed-0.1.99/meshed/composition.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/dag.py` & `meshed-0.1.99/meshed/dag.py`

 * *Files 12% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 """
 
 from functools import partial, wraps, cached_property
 from collections import defaultdict
 
 from dataclasses import dataclass, field
 from itertools import chain
-from operator import attrgetter
+from operator import attrgetter, eq
 from typing import (
     Callable,
     MutableMapping,
     Union,
     Optional,
     Iterable,
     Any,
@@ -155,24 +155,27 @@
 from i2.signatures import (
     call_somewhat_forgivingly,
     call_forgivingly,
     Parameter,
     empty,
     Sig,
     sort_params,
+    # SignatureComparator,
+    CallableComparator,
 )
 from meshed.base import (
     FuncNode,
     ch_func_node_func,
     validate_that_func_node_names_are_sane,
     _mk_func_nodes,
     _func_nodes_to_graph_dict,
     is_func_node,
     FuncNodeAble,
     func_node_transformer,
+    compare_signatures,
 )
 
 from meshed.util import (
     lambda_name,
     ValidationError,
     NotUniqueError,
     NotFound,
@@ -950,15 +953,22 @@
         >>> def h(a, b, g): return f"{a=} {b=} {g=}"
         >>> extended_dag = DAG([*dag, h])
         >>> extended_dag(a=2, b=3)
         'a=2 b=3 g=7'
         """
         yield from self.func_nodes
 
-    def ch_funcs(self, **func_mapping: Callable):
+    # Note: signature_comparator is position only to not conflict with any of the
+    #  func_mapping keys.
+    def ch_funcs(
+        self,
+        func_comparator: CallableComparator = compare_signatures,
+        /,
+        **func_mapping: Callable,
+    ) -> 'DAG':
         """
         Change some of the functions in the DAG.
         More preciseluy get a copy of the DAG where in some of the functions have
         changed.
 
         :param name_and_func: ``name=func`` pairs where ``name`` is the
             ``FuncNode.name`` of the func nodes you want to change and func is the
@@ -985,16 +995,104 @@
         15
         >>> dd = d.ch_funcs(f=lambda a, b: a - b)
         >>> dd(2, 3)  # (2 - 3) * 3 == -1 * 3
         -3
 
         You can reference the ``FuncNode`` you want to change through its ``.name`` or
         ``.out`` attribute (both are unique to this ``FuncNode`` in a ``DAG``).
+
+        >>> from i2 import Sig
+        >>>
+        >>> dag = DAG([
+        ...     FuncNode(lambda a, b: a + b, name='f'),
+        ...     FuncNode(lambda y=1, z=2: y * z, name='g', bind={'z': 'f'})
+        ... ])
+        >>>
+        >>> Sig(dag)
+        <Sig (a, b, f=2, y=1)>
+        >>>
+
+        If you replace by a different function with exactly the same signature,
+        all goes well:
+
+        >>> dag.ch_funcs(g=lambda y=1, z=2: y / z)
+        DAG(func_nodes=[FuncNode(a,b -> f -> _f), FuncNode(z=_f,y -> g -> _g)], name=None)
+
+        But if you change the signature, even slightly you get an error.
+
+        Here we didn't include the defaults:
+
+        >>> dag.ch_funcs(g=lambda y, z: y / z)  # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
+        Traceback (most recent call last):
+          ...
+        ValueError: You can only change the func of a FuncNode with a another func if the signatures match.
+          ...
+
+        Here we include defaults, but ``z``'s is different:
+
+        >>> dag.ch_funcs(g=lambda y=1, z=200: y / z)  # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
+        Traceback (most recent call last):
+          ...
+        ValueError: You can only change the func of a FuncNode with a another func if the signatures match.
+          ...
+
+        Here the defaults are exactly the same, but the order of parameters is
+        different:
+
+        >>> dag.ch_funcs(g=lambda z=2, y=1: y / z)  # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
+        Traceback (most recent call last):
+          ...
+        ValueError: You can only change the func of a FuncNode with a another func if the signatures match.
+          ...
+
+        This validation of the functions controlled by the ``func_comparator``
+        argument. By default this is the ``compare_signatures`` which compares the
+        signatures of the functions in the strictest way possible.
+        The is the right choice for a default since it will get you out of trouble
+        down the line.
+
+        But it's also annoying in many situations, and in those cases you should
+        specify the ``func_comparator`` that makes sense for your context.
+
+        Since most of the time, you'll want to compare functions solely based on
+        their signature, we provide a ``compare_signatures`` allows you to control the
+        signature comparison through a ``signature_comparator`` argument.
+
+        >>> from meshed import compare_signatures
+        >>> from functools import partial
+        >>> on_names = lambda sig1, sig2: list(sig1.parameters) == list(sig2.parameters)
+        >>> same_names = partial(compare_signatures, signature_comparator=on_names)
+        >>> d = dag.ch_funcs(same_names, g=lambda y, z: y / z);
+        >>> Sig(d)
+        <Sig (a, b, y)>
+        >>> d(2, 3, 4)
+        0.8
+
+        And this one works too:
+
+        >>> d = dag.ch_funcs(same_names, g=lambda y=1, z=200: y / z);
+
+        But our ``same_names`` function compared names including their order.
+        If we want a function with the signature ``(z=2, y=1)`` to be able to be
+        "injected" we'll need a different comparator:
+
+        >>> _names = lambda sig1, sig2: set(sig1.parameters) == set(sig2.parameters)
+        >>> same_set_of_names = partial(
+        ...     compare_signatures,
+        ...     signature_comparator=(
+        ...         lambda sig1, sig2: set(sig1.parameters) == set(sig2.parameters)
+        ...     )
+        ... )
+        >>> d = dag.ch_funcs(same_set_of_names, g=lambda z=2, y=1: y / z);
+
+
         """
-        return ch_funcs(self, func_mapping=func_mapping,)
+        return ch_funcs(
+            self, func_mapping=func_mapping, func_comparator=func_comparator
+        )
 
         # _validate_func_mapping(func_mapping, self)
         #
         # # def validate(func_mapping, func_nodes):
         #
         # # def ch_func(dag, key, func):
         # #     return DAG(
@@ -1684,16 +1782,21 @@
 # TODO: Make it work with any FuncNode Iterable
 # TODO: extract egress functionality to decorator?
 @double_up_as_factory
 def ch_funcs(
     func_nodes: DagAble = None,
     *,
     func_mapping: FuncMapping = (),
-    ch_func_node_func: Callable[[FuncNode, Callable], FuncNode] = ch_func_node_func,
     validate_func_mapping: Optional[FuncMappingValidator] = _validate_func_mapping,
+    # TODO: Design. Don't like the fact that ch_func_node_func needs a slot for
+    #  func_comparator, which is then given later.
+    ch_func_node_func: Callable[
+        [FuncNode, Callable, CallableComparator], FuncNode
+    ] = ch_func_node_func,
+    func_comparator: CallableComparator = compare_signatures,
 ):
     """Function (and decorator) to change the functions of func_nodes according to
     the specification of a func_mapping whose keys are ``.name`` or ``.out`` values
     of the nodes of ``func_nodes`` and the values are the callable we want to replace
     them by.
 
     A constrained version of ``ch_funcs`` is used as a method of ``DAG``.
@@ -1713,19 +1816,21 @@
     #             condition=lambda fn: dag._func_node_for.get(key, None) is not None,
     #             replacement=lambda fn: ch_func_node_func(fn, func=func),
     #         )
     #     )
 
     # TODO: Optimize (for example, use self._func_node_for)
     def ch_func(dag, key, func):
+        condition = lambda fn: fn.name == key or fn.out == key  # TODO: interface ctrl?
+        replacement = lambda fn: ch_func_node_func(
+            fn, func, func_comparator=func_comparator
+        )
         return DAG(
             replace_item_in_iterable(
-                dag.func_nodes,
-                condition=lambda fn: fn.name == key or fn.out == key,
-                replacement=lambda fn: ch_func_node_func(fn, func),
+                dag.func_nodes, condition=condition, replacement=replacement,
             )
         )
 
     new_dag = DAG(func_nodes)
     for key, func in func_mapping.items():
         new_dag = ch_func(new_dag, key, func)
     return new_dag
```

### Comparing `meshed-0.1.98/meshed/examples/online_marketing.py` & `meshed-0.1.99/meshed/examples/online_marketing.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/examples/price_elasticity.py` & `meshed-0.1.99/meshed/examples/price_elasticity.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/examples/vaccine_vs_no_vaccine.py` & `meshed-0.1.99/meshed/examples/vaccine_vs_no_vaccine.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/ext/gk.py` & `meshed-0.1.99/meshed/ext/gk.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/ext/gk_tests.py` & `meshed-0.1.99/meshed/ext/gk_tests.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/itools.py` & `meshed-0.1.99/meshed/itools.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/makers.py` & `meshed-0.1.99/meshed/makers.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/scrap/cached_dag.py` & `meshed-0.1.99/meshed/scrap/cached_dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     It's also okay to write into an existing key if the value it holds is identical.
     In fact, the write doesn't even happen.
 
     >>> d['b'] = 2
 
     But if we try to write a different value...
 
-    >>> d['b'] = 22
+    >>> d['b'] = 22  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     cached_dag.OverWritesNotAllowedError: The b key already exists and you're not allowed to change its value
 
     """
 
     def __setitem__(self, key, value):
```

### Comparing `meshed-0.1.98/meshed/scrap/dask_graph_language.py` & `meshed-0.1.99/meshed/scrap/dask_graph_language.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/scrap/gk_with_networkx.py` & `meshed-0.1.99/meshed/scrap/gk_with_networkx.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/scrap/wrapping_dags.py` & `meshed-0.1.99/meshed/scrap/wrapping_dags.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/objects_for_testing.py` & `meshed-0.1.99/meshed/tests/objects_for_testing.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_base.py` & `meshed-0.1.99/meshed/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_caching.py` & `meshed-0.1.99/meshed/tests/test_caching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for caching module"""
 
 
 def test_lazy_props():
     # Note: LazyProps isn't used at the time of writing this (2022-05-20) so if
     # test fails can (maybe) remove.
     from meshed.caching import LazyProps
-    from i2 import Literal
+    from i2 import LiteralVal
 
     # TODO: Why doesn't it work with dataclasses?
     # from dataclasses import dataclass
     # @dataclass
     class Funnel(LazyProps):
         #     impressions: int = 1000,
         #     cost_per_impression: float = 0.001,
@@ -42,15 +42,15 @@
 
         def revenue(self):
             return self.sales * self.revenue_per_sale
 
         def profit(self):
             return self.revenue - self.cost
 
-        @Literal  # Meaning "leave this attribute as is (i.e. don't make it a lazy prop)"
+        @LiteralVal  # Meaning "leave this attribute as is (i.e. don't make it a lazy prop)"
         def leave_this_alone(self, a, b):
             return a + b
 
     f = Funnel(impressions=100, sales_per_click=0.15)
     assert f.revenue == 30.0
     assert f.leave_this_alone(1, 2) == 3
```

### Comparing `meshed-0.1.98/meshed/tests/test_ch_funcs.py` & `meshed-0.1.99/meshed/tests/test_ch_funcs.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_dag.py` & `meshed-0.1.99/meshed/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_dag_2.py` & `meshed-0.1.99/meshed/tests/test_dag_2.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_dag_defaults.py` & `meshed-0.1.99/meshed/tests/test_dag_defaults.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_dag_variadics.py` & `meshed-0.1.99/meshed/tests/test_dag_variadics.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_getitem.py` & `meshed-0.1.99/meshed/tests/test_getitem.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_itools.py` & `meshed-0.1.99/meshed/tests/test_itools.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_makers.py` & `meshed-0.1.99/meshed/tests/test_makers.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/test_util.py` & `meshed-0.1.99/meshed/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/tests/utils_for_testing.py` & `meshed-0.1.99/meshed/tests/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `meshed-0.1.98/meshed/util.py` & `meshed-0.1.99/meshed/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """util functions"""
 import re
 from functools import partial, wraps
 from inspect import Parameter
 from typing import Callable, Any, Union, Iterator, Optional, Iterable, Mapping, TypeVar
 
-from i2 import Sig, name_of_obj, Literal, FuncFanout, Pipe
+from i2 import Sig, name_of_obj, LiteralVal, FuncFanout, Pipe
 from operator import itemgetter
 
 T = TypeVar('T')
 
 
 def if_then_else(if_func, then_func, else_func, *args, **kwargs):
     """
@@ -701,14 +701,15 @@
     return x == val
 
 
 def _not_callable(obj):
     return not callable(obj)
 
 
+# Pattern: routing
 # TODO: Replace
 def conditional_trans(
     obj: T, condition: Callable[[T], bool], trans: Callable[[T], Any]
 ):
     """Conditionally transform an object unless it is marked as a literal.
 
     >>> from functools import partial
@@ -720,21 +721,21 @@
     >>> trans('10')
     10.0
 
     To use this function but tell it to not transform some a specific input no matter
     what, wrap the input with ``Literal``
 
     >>> # from meshed import Literal
-    >>> conditional_trans(Literal('10'), str.isnumeric, float)
+    >>> conditional_trans(LiteralVal('10'), str.isnumeric, float)
     '10'
 
     """
     # TODO: Maybe make Literal checking less sensitive to isinstance checks, using
     #   hasattr instead for example.
-    if isinstance(obj, Literal):  # If val is a Literal, return its value as is
+    if isinstance(obj, LiteralVal):  # If val is a Literal, return its value as is
         return obj.val
     elif condition(obj):  # If obj satisfies condition, return the alternative_obj
         return trans(obj)
     else:  # If not, just return object
         return obj
```

### Comparing `meshed-0.1.98/meshed.egg-info/PKG-INFO` & `meshed-0.1.99/meshed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshed
-Version: 0.1.98
+Version: 0.1.99
 Summary: Link functions up into callable objects
 Home-page: https://github.com/i2mint/meshed
 License: mit
 Description: # meshed
         
         Link functions up into callable objects (e.g. pipelines, DAGs, etc.)
```

### Comparing `meshed-0.1.98/meshed.egg-info/SOURCES.txt` & `meshed-0.1.99/meshed.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 meshed/__init__.py
 meshed/base.py
 meshed/caching.py
 meshed/composition.py
 meshed/dag.py
 meshed/itools.py
 meshed/makers.py
+meshed/slabs.py
 meshed/util.py
 meshed.egg-info/PKG-INFO
 meshed.egg-info/SOURCES.txt
 meshed.egg-info/dependency_links.txt
 meshed.egg-info/not-zip-safe
 meshed.egg-info/requires.txt
 meshed.egg-info/top_level.txt
@@ -21,14 +22,15 @@
 meshed/examples/price_elasticity.py
 meshed/examples/vaccine_vs_no_vaccine.py
 meshed/ext/__init__.py
 meshed/ext/gk.py
 meshed/ext/gk_tests.py
 meshed/scrap/__init__.py
 meshed/scrap/cached_dag.py
+meshed/scrap/conversion.py
 meshed/scrap/dask_graph_language.py
 meshed/scrap/gk_with_networkx.py
 meshed/scrap/misc_utils.py
 meshed/scrap/wrapping_dags.py
 meshed/tests/__init__.py
 meshed/tests/objects_for_testing.py
 meshed/tests/test_base.py
```

