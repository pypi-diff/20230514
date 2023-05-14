# Comparing `tmp/pygim_common-0.1.0-py3-none-any.whl.zip` & `tmp/pygim_common-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,149 +1,52 @@
-Zip file size: 307881 bytes, number of entries: 147
--rw-r--r--  2.0 unx      337 b- defN 16-Jan-01 00:00 pygim/__init__.py
+Zip file size: 34732 bytes, number of entries: 50
+-rw-r--r--  2.0 unx       66 b- defN 16-Jan-01 00:00 _pygim/__init__.py
+-rw-r--r--  2.0 unx      139 b- defN 16-Jan-01 00:00 _pygim/_cli/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 16-Jan-01 00:00 _pygim/_cli/__init__.pyi
+-rw-r--r--  2.0 unx     1492 b- defN 16-Jan-01 00:00 _pygim/_cli/cliapp.py
+-rw-r--r--  2.0 unx      209 b- defN 16-Jan-01 00:00 _pygim/_cli/support.py
+-rw-r--r--  2.0 unx      102 b- defN 16-Jan-01 00:00 _pygim/_magic/__init__.py
+-rw-r--r--  2.0 unx     5128 b- defN 16-Jan-01 00:00 _pygim/_magic/_cached_type.py
+-rw-r--r--  2.0 unx     3461 b- defN 16-Jan-01 00:00 _pygim/_magic/_dispatcher.py
+-rw-r--r--  2.0 unx     6673 b- defN 16-Jan-01 00:00 _pygim/_magic/_gimmick.py
+-rw-r--r--  2.0 unx     7985 b- defN 16-Jan-01 00:00 _pygim/_magic/_patch.py
+-rw-r--r--  2.0 unx      284 b- defN 16-Jan-01 00:00 _pygim/_magic/_support.py
+-rw-r--r--  2.0 unx     1931 b- defN 16-Jan-01 00:00 _pygim/_magic/_traits.py
+-rw-r--r--  2.0 unx      337 b- defN 16-Jan-01 00:00 _pygim/_utils/__init__.py
+-rw-r--r--  2.0 unx     3933 b- defN 16-Jan-01 00:00 _pygim/_utils/_inspect.py
+-rw-r--r--  2.0 unx     2975 b- defN 16-Jan-01 00:00 _pygim/_utils/_iterable.py
+-rw-r--r--  2.0 unx      662 b- defN 16-Jan-01 00:00 pygim/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pygim/__init__.pyi
--rw-r--r--  2.0 unx      935 b- defN 16-Jan-01 00:00 pygim/__main__.py
--rw-r--r--  2.0 unx      213 b- defN 16-Jan-01 00:00 pygim/__main__.pyi
+-rw-r--r--  2.0 unx     1087 b- defN 16-Jan-01 00:00 pygim/__main__.py
+-rw-r--r--  2.0 unx      215 b- defN 16-Jan-01 00:00 pygim/__main__.pyi
 -rw-r--r--  2.0 unx       85 b- defN 16-Jan-01 00:00 pygim/__version__.py
--rw-r--r--  2.0 unx      139 b- defN 16-Jan-01 00:00 pygim/_cli/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 16-Jan-01 00:00 pygim/_cli/__init__.pyi
--rw-r--r--  2.0 unx     1280 b- defN 16-Jan-01 00:00 pygim/_cli/cliapp.py
--rw-r--r--  2.0 unx      167 b- defN 16-Jan-01 00:00 pygim/_cli/cliapp.pyi
--rw-r--r--  2.0 unx      209 b- defN 16-Jan-01 00:00 pygim/_cli/support.py
--rw-r--r--  2.0 unx       55 b- defN 16-Jan-01 00:00 pygim/_cli/support.pyi
 -rw-r--r--  2.0 unx      450 b- defN 16-Jan-01 00:00 pygim/exceptions.py
 -rw-r--r--  2.0 unx      161 b- defN 16-Jan-01 00:00 pygim/exceptions.pyi
--rw-r--r--  2.0 unx       69 b- defN 16-Jan-01 00:00 pygim/kernel/__init__.py
+-rw-r--r--  2.0 unx       78 b- defN 16-Jan-01 00:00 pygim/kernel/__init__.py
 -rw-r--r--  2.0 unx       75 b- defN 16-Jan-01 00:00 pygim/kernel/__init__.pyi
--rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 pygim/kernel/magic/__init__.py
--rw-r--r--  2.0 unx     5128 b- defN 16-Jan-01 00:00 pygim/kernel/magic/cached_type.py
+-rw-r--r--  2.0 unx     6735 b- defN 16-Jan-01 00:00 pygim/kernel/entangled_class.py
+-rw-r--r--  2.0 unx      780 b- defN 16-Jan-01 00:00 pygim/kernel/entangled_class.pyi
+-rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pygim/kernel/magic/__init__.py
 -rw-r--r--  2.0 unx     1319 b- defN 16-Jan-01 00:00 pygim/kernel/magic/cached_type.pyi
--rw-r--r--  2.0 unx     6721 b- defN 16-Jan-01 00:00 pygim/kernel/magic/entangled_class.py
--rw-r--r--  2.0 unx      780 b- defN 16-Jan-01 00:00 pygim/kernel/magic/entangled_class.pyi
--rw-r--r--  2.0 unx      284 b- defN 16-Jan-01 00:00 pygim/kernel/magic/support.py
 -rw-r--r--  2.0 unx      224 b- defN 16-Jan-01 00:00 pygim/kernel/magic/support.pyi
--rw-r--r--  2.0 unx     9452 b- defN 16-Jan-01 00:00 pygim/kernel/pathset.py
+-rw-r--r--  2.0 unx     9973 b- defN 16-Jan-01 00:00 pygim/kernel/pathset.py
 -rw-r--r--  2.0 unx     1506 b- defN 16-Jan-01 00:00 pygim/kernel/pathset.pyi
+-rw-r--r--  2.0 unx      109 b- defN 16-Jan-01 00:00 pygim/kernel/traits.py
 -rw-r--r--  2.0 unx     1241 b- defN 16-Jan-01 00:00 pygim/typing.py
--rw-r--r--  2.0 unx       34 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/.gitignore
--rw-r--r--  2.0 unx        2 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/@plugins_snapshot.json
--rw-r--r--  2.0 unx   113556 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/_ast.data.json
--rw-r--r--  2.0 unx     1627 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/_ast.meta.json
--rw-r--r--  2.0 unx    10032 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/_collections_abc.data.json
--rw-r--r--  2.0 unx     1601 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/_collections_abc.meta.json
--rw-r--r--  2.0 unx    12577 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/_compression.data.json
--rw-r--r--  2.0 unx     1557 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/_compression.meta.json
--rw-r--r--  2.0 unx    74000 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/_typeshed/__init__.data.json
--rw-r--r--  2.0 unx     1682 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/_typeshed/__init__.meta.json
--rw-r--r--  2.0 unx    19407 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/abc.data.json
--rw-r--r--  2.0 unx     1569 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/abc.meta.json
--rw-r--r--  2.0 unx    62612 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/array.data.json
--rw-r--r--  2.0 unx     1587 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/array.meta.json
--rw-r--r--  2.0 unx   947697 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/builtins.data.json
--rw-r--r--  2.0 unx     1712 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/builtins.meta.json
--rw-r--r--  2.0 unx    19912 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/cProfile.data.json
--rw-r--r--  2.0 unx     1608 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/cProfile.meta.json
--rw-r--r--  2.0 unx   127091 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/codecs.data.json
--rw-r--r--  2.0 unx     1605 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/codecs.meta.json
--rw-r--r--  2.0 unx   322905 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/collections/__init__.data.json
--rw-r--r--  2.0 unx     1611 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/collections/__init__.meta.json
--rw-r--r--  2.0 unx     4014 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/collections/abc.data.json
--rw-r--r--  2.0 unx     1516 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/collections/abc.meta.json
--rw-r--r--  2.0 unx    86654 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/contextlib.data.json
--rw-r--r--  2.0 unx     1612 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/contextlib.meta.json
--rw-r--r--  2.0 unx   128712 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/ctypes/__init__.data.json
--rw-r--r--  2.0 unx     1646 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/ctypes/__init__.meta.json
--rw-r--r--  2.0 unx     7769 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/__init__.data.json
--rw-r--r--  2.0 unx     1594 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/__init__.meta.json
--rw-r--r--  2.0 unx    12285 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/charset.data.json
--rw-r--r--  2.0 unx     1544 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/charset.meta.json
--rw-r--r--  2.0 unx     8061 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/contentmanager.data.json
--rw-r--r--  2.0 unx     1565 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/contentmanager.meta.json
--rw-r--r--  2.0 unx    24104 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/errors.data.json
--rw-r--r--  2.0 unx     1551 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/errors.meta.json
--rw-r--r--  2.0 unx     8787 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/header.data.json
--rw-r--r--  2.0 unx     1539 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/header.meta.json
--rw-r--r--  2.0 unx    55952 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/message.data.json
--rw-r--r--  2.0 unx     1747 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/message.meta.json
--rw-r--r--  2.0 unx    31215 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/policy.data.json
--rw-r--r--  2.0 unx     1637 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/email/policy.meta.json
--rw-r--r--  2.0 unx    61026 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/enum.data.json
--rw-r--r--  2.0 unx     1665 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/enum.meta.json
--rw-r--r--  2.0 unx   127134 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/functools.data.json
--rw-r--r--  2.0 unx     1611 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/functools.meta.json
--rw-r--r--  2.0 unx    19075 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/genericpath.data.json
--rw-r--r--  2.0 unx     1598 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/genericpath.meta.json
--rw-r--r--  2.0 unx    48903 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/gzip.data.json
--rw-r--r--  2.0 unx     1610 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/gzip.meta.json
--rw-r--r--  2.0 unx    27077 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/hashlib.data.json
--rw-r--r--  2.0 unx     1656 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/hashlib.meta.json
--rw-r--r--  2.0 unx     6245 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/importlib/__init__.data.json
--rw-r--r--  2.0 unx     1582 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/importlib/__init__.meta.json
--rw-r--r--  2.0 unx    44413 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/importlib/abc.data.json
--rw-r--r--  2.0 unx     1730 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/importlib/abc.meta.json
--rw-r--r--  2.0 unx    66430 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/importlib/machinery.data.json
--rw-r--r--  2.0 unx     1677 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/importlib/machinery.meta.json
--rw-r--r--  2.0 unx    65872 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/importlib/metadata/__init__.data.json
--rw-r--r--  2.0 unx     1671 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/importlib/metadata/__init__.meta.json
--rw-r--r--  2.0 unx    86160 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/io.data.json
--rw-r--r--  2.0 unx     1626 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/io.meta.json
--rw-r--r--  2.0 unx    28029 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/mmap.data.json
--rw-r--r--  2.0 unx     1558 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/mmap.meta.json
--rw-r--r--  2.0 unx   332879 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/os/__init__.data.json
--rw-r--r--  2.0 unx     1750 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/os/__init__.meta.json
--rw-r--r--  2.0 unx     5293 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/os/path.data.json
--rw-r--r--  2.0 unx     1539 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/os/path.meta.json
--rw-r--r--  2.0 unx    83881 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pathlib.data.json
--rw-r--r--  2.0 unx     1636 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pathlib.meta.json
--rw-r--r--  2.0 unx    47468 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pickle.data.json
--rw-r--r--  2.0 unx     1637 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pickle.meta.json
--rw-r--r--  2.0 unx    71997 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/posixpath.data.json
--rw-r--r--  2.0 unx     1603 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/posixpath.meta.json
--rw-r--r--  2.0 unx    18909 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/profile.data.json
--rw-r--r--  2.0 unx     1577 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/profile.meta.json
--rw-r--r--  2.0 unx    30382 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pstats.data.json
--rw-r--r--  2.0 unx     1704 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pstats.meta.json
--rw-r--r--  2.0 unx     1569 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/__init__.data.json
--rw-r--r--  2.0 unx     1481 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/__init__.meta.json
--rw-r--r--  2.0 unx    16125 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/typing.data.json
--rw-r--r--  2.0 unx     1570 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/typing.meta.json
--rw-r--r--  2.0 unx     3098 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/utils/__init__.data.json
--rw-r--r--  2.0 unx     1640 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/utils/__init__.meta.json
--rw-r--r--  2.0 unx     4968 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/utils/performance.data.json
--rw-r--r--  2.0 unx     1620 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/utils/performance.meta.json
--rw-r--r--  2.0 unx     5907 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/utils/persistence.data.json
--rw-r--r--  2.0 unx     1690 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/utils/persistence.meta.json
--rw-r--r--  2.0 unx     5758 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/utils/security.data.json
--rw-r--r--  2.0 unx     1672 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/pygim/utils/security.meta.json
--rw-r--r--  2.0 unx   145965 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/subprocess.data.json
--rw-r--r--  2.0 unx     1691 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/subprocess.meta.json
--rw-r--r--  2.0 unx   137555 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/sys.data.json
--rw-r--r--  2.0 unx     1670 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/sys.meta.json
--rw-r--r--  2.0 unx    42512 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/time.data.json
--rw-r--r--  2.0 unx     1560 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/time.meta.json
--rw-r--r--  2.0 unx   228645 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/types.data.json
--rw-r--r--  2.0 unx     1664 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/types.meta.json
--rw-r--r--  2.0 unx   491666 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/typing.data.json
--rw-r--r--  2.0 unx     1650 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/typing.meta.json
--rw-r--r--  2.0 unx    49609 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/typing_extensions.data.json
--rw-r--r--  2.0 unx     1559 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/typing_extensions.meta.json
--rw-r--r--  2.0 unx    17257 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/zlib.data.json
--rw-r--r--  2.0 unx     1576 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/3.8/zlib.meta.json
--rw-r--r--  2.0 unx      190 b- defN 16-Jan-01 00:00 pygim/utils/.mypy_cache/CACHEDIR.TAG
--rw-r--r--  2.0 unx     1097 b- defN 16-Jan-01 00:00 pygim/utils/__init__.py
+-rw-r--r--  2.0 unx     1607 b- defN 16-Jan-01 00:00 pygim/utils/__init__.py
 -rw-r--r--  2.0 unx      297 b- defN 16-Jan-01 00:00 pygim/utils/__init__.pyi
--rw-r--r--  2.0 unx     1565 b- defN 16-Jan-01 00:00 pygim/utils/iterable.py
 -rw-r--r--  2.0 unx      290 b- defN 16-Jan-01 00:00 pygim/utils/iterable.pyi
--rw-r--r--  2.0 unx      354 b- defN 16-Jan-01 00:00 pygim/utils/misc.py
--rw-r--r--  2.0 unx     1346 b- defN 16-Jan-01 00:00 pygim/utils/performance.py
+-rw-r--r--  2.0 unx      513 b- defN 16-Jan-01 00:00 pygim/utils/misc.py
+-rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 pygim/utils/misc.pyi
+-rw-r--r--  2.0 unx     2385 b- defN 16-Jan-01 00:00 pygim/utils/performance.py
 -rw-r--r--  2.0 unx      256 b- defN 16-Jan-01 00:00 pygim/utils/performance.pyi
--rw-r--r--  2.0 unx     2510 b- defN 16-Jan-01 00:00 pygim/utils/persistence.py
+-rw-r--r--  2.0 unx     3954 b- defN 16-Jan-01 00:00 pygim/utils/persistence.py
 -rw-r--r--  2.0 unx      374 b- defN 16-Jan-01 00:00 pygim/utils/persistence.pyi
--rw-r--r--  2.0 unx      968 b- defN 16-Jan-01 00:00 pygim/utils/security.py
+-rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 pygim/utils/security.py
 -rw-r--r--  2.0 unx      112 b- defN 16-Jan-01 00:00 pygim/utils/security.pyi
--rw-r--r--  2.0 unx     1319 b- defN 16-Jan-01 00:00 pygim/utils/testing.py
+-rw-r--r--  2.0 unx     2448 b- defN 16-Jan-01 00:00 pygim/utils/testing.py
 -rw-r--r--  2.0 unx      334 b- defN 16-Jan-01 00:00 pygim/utils/testing.pyi
--rw-r--r--  2.0 unx     2004 b- defN 16-Jan-01 00:00 pygim_common-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       87 b- defN 16-Jan-01 00:00 pygim_common-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 16-Jan-01 00:00 pygim_common-0.1.0.dist-info/entry_points.txt
-?rw-------  2.0 unx    14526 b- defN 16-Jan-01 00:00 pygim_common-0.1.0.dist-info/RECORD
-147 files, 4540397 bytes uncompressed, 284299 bytes compressed:  93.7%
+-rw-r--r--  2.0 unx     2160 b- defN 16-Jan-01 00:00 pygim_common-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       87 b- defN 16-Jan-01 00:00 pygim_common-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 16-Jan-01 00:00 pygim_common-0.2.0.dist-info/entry_points.txt
+?rw-------  2.0 unx     3996 b- defN 16-Jan-01 00:00 pygim_common-0.2.0.dist-info/RECORD
+50 files, 79573 bytes uncompressed, 28428 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,412 +1,121 @@
-Filename: pygim/__init__.py
-Comment: 
-
-Filename: pygim/__init__.pyi
-Comment: 
-
-Filename: pygim/__main__.py
-Comment: 
-
-Filename: pygim/__main__.pyi
-Comment: 
-
-Filename: pygim/__version__.py
-Comment: 
-
-Filename: pygim/_cli/__init__.py
-Comment: 
-
-Filename: pygim/_cli/__init__.pyi
-Comment: 
-
-Filename: pygim/_cli/cliapp.py
-Comment: 
-
-Filename: pygim/_cli/cliapp.pyi
-Comment: 
-
-Filename: pygim/_cli/support.py
-Comment: 
-
-Filename: pygim/_cli/support.pyi
-Comment: 
-
-Filename: pygim/exceptions.py
-Comment: 
-
-Filename: pygim/exceptions.pyi
-Comment: 
-
-Filename: pygim/kernel/__init__.py
-Comment: 
-
-Filename: pygim/kernel/__init__.pyi
-Comment: 
-
-Filename: pygim/kernel/magic/__init__.py
-Comment: 
-
-Filename: pygim/kernel/magic/cached_type.py
-Comment: 
-
-Filename: pygim/kernel/magic/cached_type.pyi
-Comment: 
-
-Filename: pygim/kernel/magic/entangled_class.py
-Comment: 
-
-Filename: pygim/kernel/magic/entangled_class.pyi
-Comment: 
-
-Filename: pygim/kernel/magic/support.py
-Comment: 
-
-Filename: pygim/kernel/magic/support.pyi
-Comment: 
-
-Filename: pygim/kernel/pathset.py
-Comment: 
-
-Filename: pygim/kernel/pathset.pyi
-Comment: 
-
-Filename: pygim/typing.py
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/.gitignore
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/@plugins_snapshot.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/_ast.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/_ast.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/_collections_abc.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/_collections_abc.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/_compression.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/_compression.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/_typeshed/__init__.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/_typeshed/__init__.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/abc.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/abc.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/array.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/array.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/builtins.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/builtins.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/cProfile.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/cProfile.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/codecs.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/codecs.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/collections/__init__.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/collections/__init__.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/collections/abc.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/collections/abc.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/contextlib.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/contextlib.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/ctypes/__init__.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/ctypes/__init__.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/__init__.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/__init__.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/charset.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/charset.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/contentmanager.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/contentmanager.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/errors.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/errors.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/header.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/header.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/message.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/message.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/policy.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/email/policy.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/enum.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/enum.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/functools.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/functools.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/genericpath.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/genericpath.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/gzip.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/gzip.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/hashlib.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/hashlib.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/importlib/__init__.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/importlib/__init__.meta.json
+Filename: _pygim/__init__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/importlib/abc.data.json
+Filename: _pygim/_cli/__init__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/importlib/abc.meta.json
+Filename: _pygim/_cli/__init__.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/importlib/machinery.data.json
+Filename: _pygim/_cli/cliapp.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/importlib/machinery.meta.json
+Filename: _pygim/_cli/support.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/importlib/metadata/__init__.data.json
+Filename: _pygim/_magic/__init__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/importlib/metadata/__init__.meta.json
+Filename: _pygim/_magic/_cached_type.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/io.data.json
+Filename: _pygim/_magic/_dispatcher.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/io.meta.json
+Filename: _pygim/_magic/_gimmick.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/mmap.data.json
+Filename: _pygim/_magic/_patch.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/mmap.meta.json
+Filename: _pygim/_magic/_support.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/os/__init__.data.json
+Filename: _pygim/_magic/_traits.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/os/__init__.meta.json
+Filename: _pygim/_utils/__init__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/os/path.data.json
+Filename: _pygim/_utils/_inspect.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/os/path.meta.json
+Filename: _pygim/_utils/_iterable.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/pathlib.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pathlib.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pickle.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pickle.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/posixpath.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/posixpath.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/profile.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/profile.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pstats.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pstats.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/__init__.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/__init__.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/typing.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/typing.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/utils/__init__.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/utils/__init__.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/utils/performance.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/utils/performance.meta.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/utils/persistence.data.json
-Comment: 
-
-Filename: pygim/utils/.mypy_cache/3.8/pygim/utils/persistence.meta.json
+Filename: pygim/__init__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/pygim/utils/security.data.json
+Filename: pygim/__init__.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/pygim/utils/security.meta.json
+Filename: pygim/__main__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/subprocess.data.json
+Filename: pygim/__main__.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/subprocess.meta.json
+Filename: pygim/__version__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/sys.data.json
+Filename: pygim/exceptions.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/sys.meta.json
+Filename: pygim/exceptions.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/time.data.json
+Filename: pygim/kernel/__init__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/time.meta.json
+Filename: pygim/kernel/__init__.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/types.data.json
+Filename: pygim/kernel/entangled_class.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/types.meta.json
+Filename: pygim/kernel/entangled_class.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/typing.data.json
+Filename: pygim/kernel/magic/__init__.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/typing.meta.json
+Filename: pygim/kernel/magic/cached_type.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/typing_extensions.data.json
+Filename: pygim/kernel/magic/support.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/typing_extensions.meta.json
+Filename: pygim/kernel/pathset.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/zlib.data.json
+Filename: pygim/kernel/pathset.pyi
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/3.8/zlib.meta.json
+Filename: pygim/kernel/traits.py
 Comment: 
 
-Filename: pygim/utils/.mypy_cache/CACHEDIR.TAG
+Filename: pygim/typing.py
 Comment: 
 
 Filename: pygim/utils/__init__.py
 Comment: 
 
 Filename: pygim/utils/__init__.pyi
 Comment: 
 
-Filename: pygim/utils/iterable.py
-Comment: 
-
 Filename: pygim/utils/iterable.pyi
 Comment: 
 
 Filename: pygim/utils/misc.py
 Comment: 
 
+Filename: pygim/utils/misc.pyi
+Comment: 
+
 Filename: pygim/utils/performance.py
 Comment: 
 
 Filename: pygim/utils/performance.pyi
 Comment: 
 
 Filename: pygim/utils/persistence.py
@@ -423,20 +132,20 @@
 
 Filename: pygim/utils/testing.py
 Comment: 
 
 Filename: pygim/utils/testing.pyi
 Comment: 
 
-Filename: pygim_common-0.1.0.dist-info/METADATA
+Filename: pygim_common-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pygim_common-0.1.0.dist-info/WHEEL
+Filename: pygim_common-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pygim_common-0.1.0.dist-info/entry_points.txt
+Filename: pygim_common-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pygim_common-0.1.0.dist-info/RECORD
+Filename: pygim_common-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pygim/__init__.py

```diff
@@ -1,15 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 Python Gimmicks Library.
 """
 
 from .__version__ import __version__
-from .kernel import *
 
 __author__ = "Teppo Perä"
 __email__ = "debith-dev@outlook.com"
 
+from .kernel import *
+from _pygim._magic._gimmick import gimmick, gim_type
+from _pygim._magic._dispatcher import dispatch
+
 __all__ = [
+    "gimmick",      # This is equivalent to Python's `object`. Inherit this!
+    "gim_type",     # This is equivalent to Python's `type`, creates `gimmick`s.
+    "dispatch",     # This is supercedes singledispatch(method).
+
     "EntangledClass",  # A class that can be shared and extended across modules.
     "PathSet",  # A class to manage multiple Path objects.
 ]
```

## pygim/__main__.py

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 Python Gimmicks Command-Line Interface.
 """
 
 import click
-from pygim._cli.cliapp import GimmicksCliApp
+from _pygim._cli.cliapp import GimmicksCliApp
 
-from pygim._cli import flag_opt
+from _pygim._cli import flag_opt
 
 
 @click.group()
 def cli():
     """\b
      ___       ___ _
     | _ \_  _ / __(_)_ __
@@ -27,7 +27,13 @@
 @flag_opt("-p", "--pycache-dirs",   help="Remove all __pycache__ folders.")
 @flag_opt("-b", "--build-dirs",     help="Remove any and all build folders.")
 @flag_opt("-c", "--compiled-files", help="Remove compiled files")
 @flag_opt("-a", "--all",            help="Remove all extra files or folders.")
 def clean_up(**kwargs):
     """ Remove unnecessary files and folders related to Python. """
     GimmicksCliApp().clean_up(**kwargs)
+
+
+@cli.command()
+def show_test_coverage(**kwargs):
+    """ Run test coverage in current folder. """
+    GimmicksCliApp().show_test_coverage(**kwargs)
```

## pygim/__main__.pyi

```diff
@@ -1,6 +1,6 @@
 from pygim.typing import AnyKwargs
-from pygim._cli import flag_opt as flag_opt
-from pygim._cli.cliapp import GimmicksCliApp as GimmicksCliApp
+from _pygim._cli import flag_opt as flag_opt
+from _pygim._cli.cliapp import GimmicksCliApp as GimmicksCliApp
 
 def cli() -> None: ...
 def clean_up(**kwargs: AnyKwargs) -> None: ...
```

## pygim/__version__.py

```diff
@@ -1,2 +1,2 @@
-__version_info__ = (0, 1, 0)
+__version_info__ = (0, 2, 0)
 __version__ = '.'.join(str(v) for v in __version_info__)
```

## pygim/kernel/__init__.py

```diff
@@ -1,4 +1,4 @@
 # -*- coding: utf-8 -*-
 
 from .pathset import *
-from .magic import *
+from .entangled_class import *
```

## pygim/kernel/magic/__init__.py

```diff
@@ -1,6 +0,0 @@
-00000000: 6672 6f6d 202e 7375 7070 6f72 7420 696d  from .support im
-00000010: 706f 7274 202a 0a66 726f 6d20 2e63 6163  port *.from .cac
-00000020: 6865 645f 7479 7065 2069 6d70 6f72 7420  hed_type import 
-00000030: 2a0a 6672 6f6d 202e 656e 7461 6e67 6c65  *.from .entangle
-00000040: 645f 636c 6173 7320 696d 706f 7274 202a  d_class import *
-00000050: 0a                                       .
```

## pygim/kernel/pathset.py

```diff
@@ -2,18 +2,16 @@
 """
 This module contains implementation of PathSet class.
 """
 
 import shutil
 from pathlib import Path
 from dataclasses import dataclass
-from typing import Iterable
 
 from pygim.utils import is_container, flatten
-import pygim.typing as t
 
 
 def _flatten_paths(paths):
     for path in flatten(paths):
         path = Path(path)
 
         if path.is_dir():
@@ -42,36 +40,35 @@
         assert isinstance(self.__pathset, PathSet)
         for p in self.__pathset:
             self.delete(p)
 
 
 @dataclass(frozen=True)
 class PathSet:
-    """This class encapsulates manipulation of multiple path objects at once.
+    """
+    This class encapsulates manipulation of multiple path objects at once.
 
     Overview (further info in function docs):
-        - len(PathSet()) provides total number of files and directories read recursively.
-        - list(PathSet()) provides list of all Path objects in the list.
-        - bool(PathSet()) tells whether there is any Path objects in the list.
-        - repr(PathSet()) provides nice string representation of this object.
-        - PathSet.prefixed()
-        - PathSet() + PathSet() creates new object contains Path objects from both sets.
-        - PathSet.prefixed() create new PathSet with another path as prefix (e.g. folder+files).
-        - PathSet().clone() creates identical copy of the list.
+        - len(PathSet()) provides the total number of files and directories read recursively.
+        - list(PathSet()) provides a list of all Path objects in the list.
+        - bool(PathSet()) tells whether there are any Path objects in the list.
+        - repr(PathSet()) provides a nice string representation of this object.
+        - PathSet.prefixed() creates a new PathSet with another path as a prefix (e.g., folder+files).
+        - PathSet() + PathSet() creates a new object containing Path objects from both sets.
+        - PathSet().clone() creates an identical copy of the list.
         - PathSet().filter() generator that yields Path objects whose properties match the filters.
         - PathSet().drop() generator that yields Path objects whose properties do NOT match the filters.
-        - PathSet().filtered() as above but returns a new PathSet object.
-        - PathSet().dirs() a shorthand for list of dirs.
-        - PathSet().files() a shorthand for list of files.
+        - PathSet().filtered() as above, but returns a new PathSet object.
+        - PathSet().dirs() a shorthand for a list of directories.
+        - PathSet().files() a shorthand for a list of files.
         - PathSet().by_suffix() a shorthand for filtering by suffix(es).
-        - PathSet().delete_all() deletes all contained Path objects from the file-system.
+        - PathSet().delete_all() deletes all contained Path objects from the file system.
 
-    TODO: This class could allow multiple different path types (not just pathlib.Path).
     """
-
+    # TODO: This class could allow multiple different path types (not just pathlib.Path).
     _paths: Path = None  # type: ignore    # this is invariant
     _pattern: str = "*"
     FS = _FileSystemOps()  # File system
 
     def __post_init__(self):
         paths = self._paths
 
@@ -83,17 +80,32 @@
 
         super().__setattr__("_paths", frozenset(_flatten_paths([paths])))
         assert all([isinstance(p, Path) for p in self._paths])
         assert isinstance(self._paths, frozenset)
 
     @classmethod
     def prefixed(cls, paths, *, prefix=None):
+        """
+        Create a new PathSet object with a specified prefix for each path.
+
+        Parameters
+        ----------
+        paths : `iterable` [path-like object]
+            Iterable of path-like objects.
+        prefix : path-like object, optional
+            The prefix to add to each path in the input `paths`. Defaults to the current working directory.
+
+        Returns
+        -------
+        PathSet
+            New PathSet object with the specified prefix for each path.
+        """
         if prefix is None:
             prefix = Path.cwd()
-        prefix = Path(prefix)  # Ensure pathlike object is Path.
+        prefix = Path(prefix)  # Ensure path-like object is Path.
 
         return cls([prefix.joinpath(p) for p in paths])
 
     def __len__(self):
         assert self._paths is not None
         return len(self._paths)
 
@@ -106,59 +118,68 @@
         return bool(self._paths)
 
     def __repr__(self):  # pragma: no cover
         assert self._paths is not None
         return f"{self.__class__.__name__}({list(str(p) for p in self._paths)})"
 
     def clone(self, paths=None):
-        """Create copy of the object.
-
-        Args:
-            paths (t.MaybePathLikes, optional):
-                Override paths in the clone. Defaults to None.
+        """
+        Create a copy of the object.
 
-        Returns:
-            PathSet: New Pathset collection.
+        Parameters
+        ----------
+        paths : `iterable` [`pathlib.Path`], optional
+            Override paths in the clone. Defaults to None.
+
+        Returns
+        -------
+        PathSet
+            New PathSet collection.
         """
         paths = self._paths if paths is None else paths
         instance = self.__class__([])
         super(self.__class__, instance).__setattr__("_paths", frozenset(Path(p) for p in paths))
         return instance
 
     def filter(self, **filters):
-        """Filter paths based on their properties, where those matching filters are kept.
+        """
+        Filter paths based on their properties, where those matching filters are kept.
 
-        Args:
-            filters (PathFilters):
-                Filters in this function has following functions:
-
-                    - KEYs must always be valid attribute names for underlying
-                      path objects. The KEY can be attribute, property or function.
-                      In case of function, the function is automatically invoked.
-                      However, functions requiring arguments are not supported.
-
-                    - VALUEs represents the expected results of corresponding
-                      attributes or return values of the functions accessed by
-                      the KEY. VALUE can be a single value, or iterable of multiple
-                      different values. For latter case, if any of the VALUEs is
-                      satisfied, the corresponding Path object qualifies.
-
-        Yields:
-            Iterator[PathGenerator]: Qualifying paths.
-
-        Examples:
-            >>> names = ["readme.txt", "readme.rst", "readme.md"]
-            >>> paths = PathSet(names)                      # A set of paths
-            >>> new_paths = paths.filter(suffix=".rst")     # Filter based on pathlib.Path.suffix property.
-            >>> [p.name for p in new_paths]                 # Show the names in filtered path set.
-            ['readme.rst']
-
-            >>> new_paths = paths.filter(suffix=[".rst", ".md"])    # This time we accept multiple suffixes.
-            >>> [p.name for p in sorted(new_paths)]                 # Show the names in filtered path set.
-            ['readme.md', 'readme.rst']
+        Parameters
+        ----------
+        filters : `dict`
+            Filters in this function have the following properties:
+
+                - KEYs must always be valid attribute names for the underlying
+                path objects. The KEY can be an attribute, property, or function.
+                In the case of a function, the function is automatically invoked.
+                However, functions requiring arguments are not supported.
+
+                - VALUEs represent the expected results of the corresponding
+                attributes or return values of the functions accessed by
+                the KEY. VALUE can be a single value or an iterable of multiple
+                different values. In the latter case, if any of the VALUEs is
+                satisfied, the corresponding Path object qualifies.
+
+        Yields
+        ------
+        `pathlib.Path`
+            Qualifying paths.
+
+        Examples
+        --------
+        >>> names = ["readme.txt", "readme.rst", "readme.md"]
+        >>> paths = PathSet(names)                      # A set of paths
+        >>> new_paths = paths.filter(suffix=".rst")     # Filter based on pathlib.Path.suffix property.
+        >>> [p.name for p in new_paths]                 # Show the names in the filtered path set.
+        ['readme.rst']
+
+        >>> new_paths = paths.filter(suffix=[".rst", ".md"])    # This time we accept multiple suffixes.
+        >>> [p.name for p in sorted(new_paths)]                 # Show the names in the filtered path set.
+        ['readme.md', 'readme.rst']
         """
         assert filters, "No filters given!"
         assert self._paths is not None
 
         for p in self._paths:
             for func, value in filters.items():
                 value = value if is_container(value) else [value]
@@ -166,58 +187,64 @@
                 obj = obj() if callable(obj) else obj
 
                 if obj in value:
                     yield p
                     break
 
     def drop(self, **filters):
-        """Filter paths based on their properties, where those NOT matching filters are kept.
+        """
+        Filter paths based on their properties, where those NOT matching filters are kept.
 
-        Args:
-            filters (PathFilters):
-                Filters in this function has following functions:
-
-                    - KEYs must always be valid attribute names for underlying
-                      path objects. The KEY can be attribute, property or function.
-                      In case of function, the function is automatically invoked.
-                      However, functions requiring arguments are not supported.
-
-                    - VALUEs represents the expected results of corresponding
-                      attributes or return values of the functions accessed by
-                      the KEY. VALUE can be a single value, or iterable of multiple
-                      different values. For latter case, if any of the VALUEs is
-                      satisfied, the corresponding Path object qualifies.
-
-        Yields:
-            Iterator[PathGenerator]: Not-Qualifying paths.
-
-        Examples:
-            >>> names = ["readme.txt", "readme.rst", "readme.md"]
-            >>> paths = PathSet(names)                      # A set of paths
-            >>> new_paths = paths.drop(suffix=".rst")       # Filter based on pathlib.Path.suffix property.
-            >>> [p.name for p in sorted(new_paths)]         # Show the names in filtered path set.
-            ['readme.md', 'readme.txt']
-
-            >>> new_paths = paths.drop(suffix=[".rst", ".md"])      # This time we accept multiple suffixes.
-            >>> [p.name for p in new_paths]                         # Show the names in filtered path set.
-            ['readme.txt']
+        Parameters
+        ----------
+        filters : `dict`
+            Filters in this function have the following properties:
+
+                - KEYs must always be valid attribute names for the underlying
+                path objects. The KEY can be an attribute, property, or function.
+                In the case of a function, the function is automatically invoked.
+                However, functions requiring arguments are not supported.
+
+                - VALUEs represent the expected results of the corresponding
+                attributes or return values of the functions accessed by
+                the KEY. VALUE can be a single value or an iterable of multiple
+                different values. In the latter case, if any of the VALUEs is
+                satisfied, the corresponding Path object qualifies.
+
+        Yields
+        ------
+        `pathlib.Path`
+            Non-qualifying paths.
+
+        Examples
+        --------
+        >>> names = ["readme.txt", "readme.rst", "readme.md"]
+        >>> paths = PathSet(names)                      # A set of paths
+        >>> new_paths = paths.drop(suffix=".rst")       # Filter based on pathlib.Path.suffix property.
+        >>> [p.name for p in sorted(new_paths)]         # Show the names in the filtered path set.
+        ['readme.md', 'readme.txt']
+
+        >>> new_paths = paths.drop(suffix=[".rst", ".md"])      # This time we accept multiple suffixes.
+        >>> [p.name for p in new_paths]                         # Show the names in the filtered path set.
+        ['readme.txt']
         """
         assert filters, "No filters given!"
         assert self._paths is not None
 
         for p in self._paths:
             for func, value in filters.items():
                 value = value if is_container(value) else [value]
                 obj = getattr(p, func)
                 obj = obj() if callable(obj) else obj
 
                 if obj not in value:
                     yield p
                     break
 
+
     def filtered(self, **filters):
         """As filter() but returns new object."""
         return self.clone(self.filter(**filters)) if filters else self
 
     def dropped(self, **filters):
         """As drop() but returns new object."""
         return self.clone(self.drop(**filters)) if filters else self
```

## pygim/utils/__init__.py

```diff
@@ -2,25 +2,30 @@
 """
 This package contains various utilities.
 
 NOTE: All the utilities here must be standalone, therefore never should
       import any modules outside from this package.
 """
 
-from .iterable import *
 from .performance import *
 from .persistence import *
 from .security import *
 from .misc import *
+from _pygim._utils import format_dict
+from _pygim._utils._iterable import split, flatten, is_container
+from _pygim._utils._inspect import has_instances, diff
 
 __all__ = [
-    "split",  # Split iterable in two iterables based on condition function.
-    "is_container",  # Check whether object is iterable but not string or bytes.
-    "flatten",  # Convert nested arrays in to a one flat array.
-    "quick_timer",  # Calculate time spent inside code within ´with´-statement.
-    "quick_profile",  # Profile code inside `with`-statement.
-    "write_bytes",  # Write bytes into a file, can ensure folder structure on write.
-    "pickle_and_compress",  # Pickle object, compress it, and optionally write to file.
     "decompress_and_unpickle",  # Decompress obj, unpickle it, while optionally read it from file.
-    "sha256sum",  # Provides sha256 for a string.
-    "safedelattr",  # Delete attribute, ignoring error when its missing.
+    "diff",                     # Compares two dictionaries and visually displays their differences.
+    "flatten",                  # Convert nested arrays in to a one flat array.
+    "format_dict",              # Function that formats dict in pretty way.
+    "has_instances",            # As `isinstance` but for objects inside iterable.
+    "is_container",             # Check whether object is iterable but not string or bytes.
+    "pickle_and_compress",      # Pickle object, compress it, and optionally write to file.
+    "quick_profile",            # Profile code inside `with`-statement.
+    "quick_timer",              # Calculate time spent inside code within ´with´-statement.
+    "safedelattr",              # Delete attribute, ignoring error when its missing.
+    "sha256sum",                # Provides sha256 for a any arguments.
+    "split",                    # Split iterable in two iterables based on condition function.
+    "write_bytes",              # Write bytes into a file, can ensure folder structure on write.
 ]
```

## pygim/utils/misc.py

```diff
@@ -3,12 +3,21 @@
 This module contains utilities not fitting to other category.
 """
 
 __all__ = ["safedelattr"]
 
 
 def safedelattr(obj, name):
-    """Deletes attribute from the object and is happy if it is not there."""
+    """Deletes attribute from the object and is happy if it is not there.
+
+    Parameters
+    ----------
+    obj : `object`
+        Object containing the attribute.
+    name : `str`
+        Name of the attribute to be deleted.
+    """
+
     try:
         delattr(obj, name)
     except AttributeError:
         pass  # It is already deleted and we are fine with it.
```

## pygim/utils/performance.py

```diff
@@ -9,50 +9,88 @@
 import time
 import pygim.typing as t
 
 __all__ = ("quick_timer", "quick_profile")
 
 
 @contextmanager
-def quick_timer(title="Code block", *, printer=print):
+def quick_timer(title: str = "Code block", *, printer=print):
     """
-    Use this function to quickly measure time on a code block.
+    Measure the execution time of a code block using a context manager.
 
-    Usage:
-    '''python
-        with quick_profile():
-            slow_code()
-    '''
+    Parameters:
+    -----------
+    title : `str`, optional
+        The title to display when printing the execution time. Default is "Code block".
+    printer : `Callable[[str], None]`, optional
+        The function to use for printing the execution time. Default is `print`.
+
+    Yields:
+    -------
+    None
+        This function is used as a context manager and doesn't return any values.
+
+    Example:
+    --------
+    Measure the time it takes to execute a loop:
+    .. code-block:: python
+
+        from time import sleep
+
+        def slow_code():
+            for i in range(10):
+                sleep(0.1)
 
-    Arguments:
-        title:      Print the time used to run code block.
+        with quick_timer(title="Slow code"):
+            slow_code()
     """
     start = time.time()
     yield
     end = time.time()
-    printer(f"{title} executed in {end-start:.2f} seconds!")
+    printer(f"{title} executed in {end - start:.2f} seconds!")
 
 
 @contextmanager
-def quick_profile(top=30, *, sort="cumtime"):
+def quick_profile(top=30, *, sort="cumtime", examine=False):
     """
-    Used to quickly print out profile results from the code inside the context.
-
-    Usage:
-    '''python
-        with quick_profile():
-            slow_code()
-    '''
+    Print profile results for code executed within a context.
 
-    Arguments:
-        top:        Print the number of the slowest functions
-        sort:       Sort functions from slowest to fastests using cumtime column
-        examine:    Enables break points of the stats are printed for further debugging.
+    Parameters
+    ----------
+    top : int, optional
+        Number of functions to print profiling results for. Default is 30.
+    sort : str, optional
+        Column to sort the profiling results by. Default is "cumtime".
+    examine : bool, optional
+        Flag indicating whether to enable breakpoints for further debugging. Default is False.
+
+    Yields
+    ------
+    None
+        This function is used as a context manager and doesn't return any values.
+
+    Example
+    -------
+    Profile the execution time of a slow loop:
+    ```python
+    def slow_code():
+        for i in range(100000):
+            pass
+
+    with quick_profile(top=5, sort="time"):
+        slow_code()
+    ```
     """
     profile = cProfile.Profile()
     profile.enable()
 
-    yield
-
-    profile.disable()
-    stats = pstats.Stats(profile).strip_dirs()
-    stats.sort_stats(sort).print_stats(top)
+    try:
+        yield
+    finally:
+        profile.disable()
+        stats = pstats.Stats(profile).strip_dirs()
+        stats.sort_stats(sort)
+        if examine:
+            stats.print_stats()
+            breakpoint()
+        else:
+            stats.print_stats(top)
```

## pygim/utils/persistence.py

```diff
@@ -15,67 +15,132 @@
 def _drop_file_suffixes(p):
     while p.suffixes:
         p = p.with_suffix("")
     return p
 
 
 def write_bytes(filename, data, *, make_dirs=False, suffix=".bin"):
-    """Writes bytes into file.
+    """
+    Write bytes data to a file.
+
+    This function provides a straightforward means of writing bytes data to a file by passing
+    the name of the file and the contents to write. It optionally creates any necessary folders
+    to allow writing.
+
+    Parameters
+    ----------
+    filename : `str`
+        Name of the file to be written.
+    data : `bytes`
+        Data to be written to the file.
+    make_dirs : `bool`, optional
+        Create any necessary folders to allow writing. Defaults to `False`.
+    suffix : `str`, optional
+        The file suffix to use when writing the file. Defaults to `.bin`.
+
+    Raises
+    ------
+    AssertionError
+        If the `data` parameter is not a bytes object or if the parent directory
+        doesn't exist and `make_dirs` is `False`.
+
+    Examples
+    --------
+    Write a bytes object to a file:
 
-    This function provides straight-forward means to write bytedata into a
-    file by passing the name of the file and the contents to write. Additionally,
-    by providing argument, it creates any necessary folders to allow writing.
-
-    Args:
-        filename (_type_): Name of the file to be written.
-        data (bytes): Data to be written in file.
-        make_dirs (bool, optional): Create folder structure. Defaults to False.
+    .. code-block:: python
+
+        data = b"Hello, world!"
+        write_bytes("hello.bin", data)
     """
-    assert isinstance(data, bytes)
-    pth: pathlib.Path = pathlib.Path(filename)
+    assert isinstance(data, bytes), "Data parameter must be a bytes object."
+
+    pth = pathlib.Path(filename)
     parent = pth.parent
 
     if make_dirs and not parent.is_dir():
         parent.mkdir(parents=True, exist_ok=True)
 
-    assert pth.parent.is_dir(), f"Parent dir does not exist for file: {str(pth.resolve())}"
+    assert parent.is_dir(), f"Parent directory doesn't exist for file: {str(pth.resolve())}"
+
     if suffix:
         pth = _drop_file_suffixes(pth).with_suffix(suffix)
-    pth.write_bytes(data)
 
+    pth.write_bytes(data)
 
-def pickle_and_compress(obj, filename=None, *, make_dirs, suffix=".pkl.zip"):
-    """Writes pickled and compressed object into a file.
 
-    Args:
-        filename (_type_): Name of the file to be written.
-        data (bytes): Data to be written in file.
-        make_dirs (bool, optional): Create folder structure. Defaults to False.
-        suffix (str, optional): File suffix used to write the file. Set as None, if
-                                you include suffix in the filename, otherwise it is
-                                replaced.
+def pickle_and_compress(obj, filename=None, *, make_dirs=False, suffix=".pkl.zip"):
+    """
+    Pickles and compresses an object, and writes it to a file.
 
-    Returns:
-        (bytes): Pickled and compressed object in bytes.
+    Parameters
+    ----------
+    obj : `object`
+        The object to be pickled and compressed.
+    filename : `str`, optional
+        Name of the file to write the pickled and compressed object to. Defaults to None,
+        which means that result is returned as bytes.
+    make_dirs : `bool`, optional
+        Create any necessary folders to allow writing. Defaults to False.
+    suffix : `str`, optional
+        The file suffix to use when writing the file. Defaults to ".pkl.zip".
+
+    Returns
+    -------
+    `bytes`
+        Pickled and compressed object in bytes.
+
+    Notes
+    -----
+    This function uses the gzip module to compress the pickled object before writing it to a file.
+
+    If `filename` is not specified, the pickled and compressed object will be returned as bytes.
+
+    Examples
+    --------
+    Pickle and compress an object and write it to a file:
+
+    .. code-block:: python
+
+        my_list = [1, 2, 3, 4, 5]
+        pickle_and_compress(my_list, filename="my_list.pkl.zip", make_dirs=True)
+
+    Pickle and compress an object and return the bytes:
+    >>> my_dict = {"name": "John", "age": 30}
+    >>> data = pickle_and_compress(my_dict)
     """
     data = gzip.compress(pickle.dumps(obj))
+
     if filename is not None:
         write_bytes(filename, data, make_dirs=make_dirs, suffix=suffix)
 
     return data
 
 
 def decompress_and_unpickle(obj):
-    """Decompress and unpickle given object.
+    """
+    Decompresses and unpickles a given object.
+
+    Parameters
+    ----------
+    obj : `str` or `pathlib.Path`
+        A byte object or a `Path` object used to read the data.
+
+    Returns
+    -------
+    `object`
+        The object returned by this procedure.
+
+    Examples
+    --------
+    Load and unpickle a compressed file:
 
-    Args:
-        obj (_type_): A byte object, or `Path` object used to read the data.
+    .. code-block:: python
 
-    Returns:
-        (object): Object returned by this procedure.
+        obj = decompress_and_unpickle("file.pkl.zip")
     """
     if isinstance(obj, str):
         pth = pathlib.Path(obj)
         if pth.is_file():
             obj = pth
 
     if isinstance(obj, pathlib.Path):
```

## pygim/utils/security.py

```diff
@@ -1,34 +1,45 @@
 # -*- coding: utf-8 -*-
 """
 This module contains security utilities.
 """
 
 import hashlib
-from functools import singledispatch
-
-import pygim.typing as t
 
+from _pygim._magic._dispatcher import dispatch
 
 __all__ = ["sha256sum"]
 
 
-@singledispatch
+@dispatch
 def sha256sum(obj, *, encoding="utf-8"):
-    """Quickly get SHA256 sum for given string.
+    """
+    Compute the SHA256 sum for the given string.
+
+    Parameters
+    ----------
+    obj : `str`
+        String to be encoded.
+    encoding : `str`, optional
+        Encoding used to convert string objects into bytes. Defaults to "utf-8".
+
+    Returns
+    -------
+    `str`
+        Calculated SHA256 sum.
+
+    Raises
+    ------
+    NotImplementedError
+        If `sha256sum` is not implemented for the given object type.
 
+    Examples
+    --------
     >>> sha256sum("hello sha256!")
     '705cb95c164e32feec2aef56f70d73e064afe2e38d40e5189fc5f8cdc84a9eaf'
-
-    Args:
-        obj (str):      String to be encoded.
-        encoding (str): Encoding used to convert string objects into bytes.
-
-    Returns:
-        Calculated SHA256 sum
     """
     raise NotImplementedError(f"sha256sum not implemented for type: {type(obj)}")
 
 
 @sha256sum.register(str)
 def _(text: str, *, encoding="utf-8"):
     assert isinstance(text, str)
```

## pygim/utils/testing.py

```diff
@@ -12,34 +12,65 @@
 __all__ = ["measure_coverage", "run_tests"]
 
 
 @contextmanager
 def measure_coverage(*, include=None, show_missing: bool = True):
     """Run code coverage for the code executed in this context manager.
 
-    Parameters:
-        include: File to be included in the coverage report. If None, all shown.
-        show_missing: True, if coverage report should include lines that were not run.
+    Parameters
+    ----------
+    include : bool, optional
+        File to be included in the coverage report. If None, all shown.
+    show_missing : bool, optional
+        True, if coverage report should include lines that were not run.
     """
     cov = coverage.Coverage()
     cov.start()
 
     yield
 
     cov.stop()
     cov.save()
     cov.report(include=include, show_missing=show_missing)
 
 
 def run_tests(test_file, module_name, pytest_args=None, *, coverage: bool = True):
-    """Runs tests for the file."""
+    """Run tests on given file.
+
+    Examples
+    --------
+    This function is typically included at the bottom of `test_<myfile>.py`.
+
+    .. code-block: python
+        if __name__ == "__main__":
+            from pygim.utils import run_tests
+            run_tests(__file__, MyClass.__module__, coverage=True)
+
+    Notes
+    -----
+    When coverage is enabled, debugging the actual code is not possible, as the module
+    must be reloaded before execution to ensure coverage for the module is captured.
+    This can remove breakpoints assigned from the IDE.
+
+    Parameters
+    ----------
+    test_file : `str` or `pathlib.Path`
+        Path to file to be tested.
+    module_name : `str`
+        Name of the module used for coverage. Usually works by passing object.__class__.__module__.
+    pytest_args : `tuple`, optional
+        Any arguments needed to be passed for pytest. (the default is None, which means default
+        argument set is given).
+    coverage : `bool`, optional
+        Runs the coverage. (the default is True, which runs the coverage).
+    """
     module = sys.modules[module_name]
-    assert isinstance(module.__file__, str)
+    assert isinstance(module.__file__, str), "No file for the module!"
 
-    pytest_args = [str(test_file), "--tb=short"]
+    pytest_args = [str(test_file), "--tb=short"] or pytest_args
 
     if not coverage:
         pytest.main(pytest_args)
         return
 
     assert module, "When running the coverage, module must be specified!"
```

## Comparing `pygim/_cli/cliapp.py` & `_pygim/_cli/cliapp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Command-Line Interface Application for Python Gimmicks.
 """
 
+import subprocess
 import sys
 from pathlib import Path
 from dataclasses import dataclass
 import click
-import pygim.typing as t
 from pygim.kernel import PathSet
 
-
 __all__ = ["GimmicksCliApp"]
 
 
 def _echo(msg, quiet):
     if not quiet:
         click.echo(msg)
 
@@ -41,7 +40,12 @@
             print("\n".join([str(n) for n in new]))
             response = input(f"Remove all {len(new)} files/folders (Y/N)? ")
             if response == "n":
                 sys.exit("No? Maybe next time...")
             elif response == "y":
                 new.FS.delete_all()
                 _echo("Excellent! You never see them again!", quiet)
+
+    def show_test_coverage(self):
+        # TODO: Make this nicer
+        subprocess.Popen("python -m coverage run -m pytest".split(' ')).wait()
+        subprocess.Popen("python -m coverage report -m".split(' ')).wait()
```

## Comparing `pygim/kernel/magic/cached_type.py` & `_pygim/_magic/_cached_type.py`

 * *Files identical despite different names*

## Comparing `pygim/kernel/magic/entangled_class.py` & `pygim/kernel/entangled_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 This creates a shared class that can be extended
 """
 
 from pygim import exceptions
 from collections.abc import Mapping, MutableMapping
-from .cached_type import CachedTypeMeta
+from _pygim._magic._cached_type import CachedTypeMeta
 
 
 __all__ = ["EntangledClass", "overrideable", "overrides"]
 
 
 def setdefaultattr(obj, name, default):
     """ Sets attribute to object in case it is missing. """
```

## Comparing `pygim/kernel/magic/entangled_class.pyi` & `pygim/kernel/entangled_class.pyi`

 * *Files identical despite different names*

## Comparing `pygim_common-0.1.0.dist-info/METADATA` & `pygim_common-0.2.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygim-common
-Version: 0.1.0
+Version: 0.2.0
 Summary: Common features for pygim
 Author: Teppo Perä
 Author-email: debith-dev@outlook.com
 Requires-Python: >=3.7, <4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,18 +18,22 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Dist: click>=8.1.3
 Requires-Dist: coverage>=6.4.4
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: pytest>=7.0.0
+Requires-Dist: tabulate>=0.8.10
 Requires-Dist: typing_extensions>=4.2.0
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: coverage[toml]; extra == "dev"
 Description-Content-Type: text/x-rst
 
 ===============================
 Python Gimmicks (pygim)
 ===============================
 
 | |docs| |downloads| |wheel| |pyversions|
```

