# Comparing `tmp/astroid-3.0.0a2.tar.gz` & `tmp/astroid-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-3.0.0a2.tar", last modified: Tue Apr 25 17:57:05 2023, max compression
+gzip compressed data, was "astroid-3.0.0a3.tar", last modified: Sun May 14 17:47:52 2023, max compression
```

## Comparing `astroid-3.0.0a2.tar` & `astroid-3.0.0a3.tar`

### file list

```diff
@@ -1,145 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.480415 astroid-3.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-25 17:56:48.000000 astroid-3.0.0a2/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-25 17:56:48.000000 astroid-3.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 17:56:48.000000 astroid-3.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 17:57:05.480415 astroid-3.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-25 17:56:48.000000 astroid-3.0.0a2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.464414 astroid-3.0.0a2/astroid/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/_backport_stdlib_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26368 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.472415 astroid-3.0.0a2/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    34564 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23321 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    45131 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.472415 astroid-3.0.0a2/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.472415 astroid-3.0.0a2/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    33517 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23500 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.476415 astroid-3.0.0a2/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (123)   134011 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.476415 astroid-3.0.0a2/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/scoped_nodes/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)   100986 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/scoped_nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.464414 astroid-3.0.0a2/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-25 17:56:48.000000 astroid-3.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 17:57:05.480415 astroid-3.0.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.480415 astroid-3.0.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_group_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)   221608 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_inference_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21514 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    61209 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_nodes_lineno.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_nodes_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_python3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_regrtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    92916 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.436113 astroid-3.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-14 17:47:37.000000 astroid-3.0.0a3/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-05-14 17:47:37.000000 astroid-3.0.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 17:47:37.000000 astroid-3.0.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-14 17:47:52.436113 astroid-3.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-14 17:47:37.000000 astroid-3.0.0a3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.424113 astroid-3.0.0a3/astroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27278 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35752 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45357 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17814 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23500 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132674 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.432113 astroid-3.0.0a3/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100964 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-14 17:47:37.000000 astroid-3.0.0a3/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.424113 astroid-3.0.0a3/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 17:47:52.000000 astroid-3.0.0a3/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-14 17:47:37.000000 astroid-3.0.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-14 17:47:37.000000 astroid-3.0.0a3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-14 17:47:37.000000 astroid-3.0.0a3/requirements_full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 17:47:37.000000 astroid-3.0.0a3/requirements_minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-14 17:47:52.436113 astroid-3.0.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:52.436113 astroid-3.0.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   221608 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61209 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92790 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-14 17:47:37.000000 astroid-3.0.0a3/tox.ini
```

### Comparing `astroid-3.0.0a2/CONTRIBUTORS.txt` & `astroid-3.0.0a3/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/LICENSE` & `astroid-3.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/PKG-INFO` & `astroid-3.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a2/README.rst` & `astroid-3.0.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/__init__.py` & `astroid-3.0.0a3/astroid/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/_ast.py` & `astroid-3.0.0a3/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/_backport_stdlib_names.py` & `astroid-3.0.0a3/astroid/_backport_stdlib_names.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/arguments.py` & `astroid-3.0.0a3/astroid/arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from __future__ import annotations
 
 from astroid import nodes
 from astroid.bases import Instance
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import InferenceError, NoDefault
 from astroid.helpers import safe_infer
+from astroid.typing import InferenceResult
 from astroid.util import Uninferable, UninferableBase
 
 
 class CallSite:
     """Class for understanding arguments passed into a call site.
 
     It needs a call context, which contains the arguments and the
@@ -130,22 +131,27 @@
                     values.append(Uninferable)
                     continue
                 values.extend(inferred.elts)
             else:
                 values.append(arg)
         return values
 
-    def infer_argument(self, funcnode, name, context):  # noqa: C901
-        """Infer a function argument value according to the call context.
+    def infer_argument(
+        self, funcnode: InferenceResult, name: str, context: InferenceContext
+    ):  # noqa: C901
+        """Infer a function argument value according to the call context."""
+        if not isinstance(funcnode, (nodes.FunctionDef, nodes.Lambda)):
+            raise InferenceError(
+                f"Can not infer function argument value for non-function node {funcnode!r}.",
+                call_site=self,
+                func=funcnode,
+                arg=name,
+                context=context,
+            )
 
-        Arguments:
-            funcnode: The function being called.
-            name: The name of the argument whose value is being inferred.
-            context: Inference context object
-        """
         if name in self.duplicated_keywords:
             raise InferenceError(
                 "The arguments passed to {func!r} have duplicate keywords.",
                 call_site=self,
                 func=funcnode,
                 arg=name,
                 context=context,
@@ -187,15 +193,15 @@
         if len(positional) < len(funcnode.args.args):
             for func_arg in funcnode.args.args:
                 if func_arg.name in kwargs:
                     arg = kwargs.pop(func_arg.name)
                     positional.append(arg)
 
         if argindex is not None:
-            boundnode = getattr(context, "boundnode", None)
+            boundnode = context.boundnode
             # 2. first argument of instance/class method
             if argindex == 0 and funcnode.type in {"method", "classmethod"}:
                 # context.boundnode is None when an instance method is called with
                 # the class, e.g. MyClass.method(obj, ...). In this case, self
                 # is the first argument.
                 if boundnode is None and funcnode.type == "method" and positional:
                     return positional[0].infer(context=context)
@@ -244,14 +250,16 @@
                     arg=name,
                     context=context,
                 )
             kwarg = nodes.Dict(
                 lineno=funcnode.args.lineno,
                 col_offset=funcnode.args.col_offset,
                 parent=funcnode.args,
+                end_lineno=funcnode.args.end_lineno,
+                end_col_offset=funcnode.args.end_col_offset,
             )
             kwarg.postinit(
                 [(nodes.const_factory(key), value) for key, value in kwargs.items()]
             )
             return iter((kwarg,))
         if funcnode.args.vararg == name:
             # It wants all the args that were passed into
```

### Comparing `astroid-3.0.0a2/astroid/astroid_manager.py` & `astroid-3.0.0a3/astroid/astroid_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/bases.py` & `astroid-3.0.0a3/astroid/bases.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """This module contains base classes and functions for the nodes and some
 inference utils.
 """
 from __future__ import annotations
 
 import collections
 import collections.abc
-from collections.abc import Iterator, Sequence
+from collections.abc import Iterable, Iterator
 from typing import TYPE_CHECKING, Any, ClassVar, Literal
 
 from astroid import nodes
 from astroid.const import PY310_PLUS
 from astroid.context import (
     CallContext,
     InferenceContext,
@@ -62,15 +62,17 @@
     "LazyProperty",
     "lazy",
     "cache_readonly",
     "DynamicClassAttribute",
 }
 
 
-def _is_property(meth, context: InferenceContext | None = None) -> bool:
+def _is_property(
+    meth: nodes.FunctionDef | UnboundMethod, context: InferenceContext | None = None
+) -> bool:
     from astroid import helpers  # pylint: disable=import-outside-toplevel
 
     decoratornames = meth.decoratornames(context=context)
     if PROPERTIES.intersection(decoratornames):
         return True
     stripped = {
         name.split(".")[-1]
@@ -88,33 +90,42 @@
         if inferred is None or isinstance(inferred, UninferableBase):
             continue
         if isinstance(inferred, nodes.ClassDef):
             for base_class in inferred.bases:
                 if not isinstance(base_class, nodes.Name):
                     continue
                 module, _ = base_class.lookup(base_class.name)
-                if module.name == "builtins" and base_class.name == "property":
+                if (
+                    isinstance(module, nodes.Module)
+                    and module.name == "builtins"
+                    and base_class.name == "property"
+                ):
                     return True
 
     return False
 
 
 class Proxy:
     """A simple proxy object.
 
     Note:
 
     Subclasses of this object will need a custom __getattr__
     if new instance attributes are created. See the Const class
     """
 
-    _proxied: nodes.ClassDef | nodes.FunctionDef
+    _proxied: nodes.ClassDef | nodes.FunctionDef | nodes.Lambda | UnboundMethod
 
     def __init__(
-        self, proxied: nodes.ClassDef | nodes.FunctionDef | None = None
+        self,
+        proxied: nodes.ClassDef
+        | nodes.FunctionDef
+        | nodes.Lambda
+        | UnboundMethod
+        | None = None,
     ) -> None:
         if proxied is None:
             # This is a hack to allow calling this __init__ during bootstrapping of
             # builtin classes and their docstrings.
             # For Const, Generator, and UnionType nodes the _proxied attribute
             # is set during bootstrapping
             # as we first need to build the ClassDef that they can proxy.
@@ -134,37 +145,39 @@
     def infer(  # type: ignore[return]
         self, context: InferenceContext | None = None, **kwargs: Any
     ) -> collections.abc.Generator[InferenceResult, None, InferenceErrorInfo | None]:
         yield self
 
 
 def _infer_stmts(
-    stmts: Sequence[InferenceResult],
+    stmts: Iterator[InferenceResult],
     context: InferenceContext | None,
     frame: nodes.NodeNG | BaseInstance | None = None,
 ) -> collections.abc.Generator[InferenceResult, None, None]:
     """Return an iterator on statements inferred by each statement in *stmts*."""
     inferred = False
     constraint_failed = False
     if context is not None:
         name = context.lookupname
         context = context.clone()
-        constraints = context.constraints.get(name, {})
+        if name is not None:
+            constraints = context.constraints.get(name, {})
+        else:
+            constraints = {}
     else:
         name = None
         constraints = {}
         context = InferenceContext()
 
     for stmt in stmts:
         if isinstance(stmt, UninferableBase):
             yield stmt
             inferred = True
             continue
-        # 'context' is always InferenceContext and Instances get '_infer_name' from ClassDef
-        context.lookupname = stmt._infer_name(frame, name)  # type: ignore[union-attr]
+        context.lookupname = stmt._infer_name(frame, name)
         try:
             stmt_constraints: set[Constraint] = set()
             for constraint_stmt, potential_constraints in constraints.items():
                 if not constraint_stmt.parent_of(stmt):
                     stmt_constraints.update(potential_constraints)
             for inf in stmt.infer(context=context):
                 if all(constraint.satisfied_by(inf) for constraint in stmt_constraints):
@@ -285,23 +298,25 @@
                 if self._proxied.__class__.__name__ != "ClassDef":
                     raise
                 attrs = self._proxied.igetattr(name, context, class_context=False)
                 yield from self._wrap_attr(attrs, context)
             except AttributeInferenceError as error:
                 raise InferenceError(**vars(error)) from error
 
-    def _wrap_attr(self, attrs, context: InferenceContext | None = None):
+    def _wrap_attr(
+        self, attrs: Iterable[InferenceResult], context: InferenceContext | None = None
+    ) -> Iterator[InferenceResult]:
         """Wrap bound methods of attrs in a InstanceMethod proxies."""
         for attr in attrs:
             if isinstance(attr, UnboundMethod):
                 if _is_property(attr):
                     yield from attr.infer_call_result(self, context)
                 else:
                     yield BoundMethod(attr, self)
-            elif hasattr(attr, "name") and attr.name == "<lambda>":
+            elif isinstance(attr, nodes.Lambda):
                 if attr.args.arguments and attr.args.arguments[0].name == "self":
                     yield BoundMethod(attr, self)
                     continue
                 yield attr
             else:
                 yield attr
 
@@ -386,15 +401,17 @@
             # Fallback to __len__.
             try:
                 result = _infer_method_result_truth(self, "__len__", context)
             except (AttributeInferenceError, InferenceError):
                 return True
         return result
 
-    def getitem(self, index, context: InferenceContext | None = None):
+    def getitem(
+        self, index: nodes.Const, context: InferenceContext | None = None
+    ) -> InferenceResult | None:
         new_context = bind_context_to_node(context, self)
         if not context:
             context = new_context
         method = next(self.igetattr("__getitem__", context=context), None)
         # Create a new CallContext for providing index as an argument.
         new_context.callcontext = CallContext(args=[index], callee=method)
         if not isinstance(method, BoundMethod):
@@ -409,33 +426,34 @@
             )
         return next(method.infer_call_result(self, new_context), None)
 
 
 class UnboundMethod(Proxy):
     """A special node representing a method not bound to an instance."""
 
-    _proxied: nodes.FunctionDef
+    _proxied: nodes.FunctionDef | UnboundMethod
 
     special_attributes: objectmodel.BoundMethodModel | objectmodel.UnboundMethodModel = (
         objectmodel.UnboundMethodModel()
     )
 
     def __repr__(self) -> str:
+        assert self._proxied.parent, "Expected a parent node"
         frame = self._proxied.parent.frame(future=True)
         return "<{} {} of {} at 0x{}".format(
             self.__class__.__name__, self._proxied.name, frame.qname(), id(self)
         )
 
     def implicit_parameters(self) -> Literal[0, 1]:
         return 0
 
     def is_bound(self) -> bool:
         return False
 
-    def getattr(self, name, context: InferenceContext | None = None):
+    def getattr(self, name: str, context: InferenceContext | None = None):
         if name in self.special_attributes:
             return [self.special_attributes.lookup(name)]
         return self._proxied.getattr(name, context)
 
     def igetattr(
         self, name: str, context: InferenceContext | None = None
     ) -> Iterator[InferenceResult]:
@@ -457,27 +475,30 @@
         the additional context (such as a classmethod) of the boundnode
         to determine which class the method was called from
         """
 
         # If we're unbound method __new__ of a builtin, the result is an
         # instance of the class given as first argument.
         if self._proxied.name == "__new__":
+            assert self._proxied.parent, "Expected a parent node"
             qname = self._proxied.parent.frame(future=True).qname()
             # Avoid checking builtins.type: _infer_type_new_call() does more validation
             if qname.startswith("builtins.") and qname != "builtins.type":
-                return self._infer_builtin_new(caller, context)
+                return self._infer_builtin_new(caller, context or InferenceContext())
         return self._proxied.infer_call_result(caller, context)
 
     def _infer_builtin_new(
         self,
-        caller: nodes.Call,
+        caller: SuccessfulInferenceResult | None,
         context: InferenceContext,
     ) -> collections.abc.Generator[
         nodes.Const | Instance | UninferableBase, None, None
     ]:
+        if not isinstance(caller, nodes.Call):
+            return
         if not caller.args:
             return
         # Attempt to create a constant
         if len(caller.args) > 1:
             value = None
             if isinstance(caller.args[1], nodes.Const):
                 value = caller.args[1].value
@@ -504,136 +525,143 @@
 
 
 class BoundMethod(UnboundMethod):
     """A special node representing a method bound to an instance."""
 
     special_attributes = objectmodel.BoundMethodModel()
 
-    def __init__(self, proxy, bound):
+    def __init__(
+        self,
+        proxy: nodes.FunctionDef | nodes.Lambda | UnboundMethod,
+        bound: SuccessfulInferenceResult,
+    ) -> None:
         super().__init__(proxy)
         self.bound = bound
 
     def implicit_parameters(self) -> Literal[0, 1]:
         if self.name == "__new__":
             # __new__ acts as a classmethod but the class argument is not implicit.
             return 0
         return 1
 
     def is_bound(self) -> Literal[True]:
         return True
 
-    def _infer_type_new_call(self, caller, context):  # noqa: C901
+    def _infer_type_new_call(
+        self, caller: nodes.Call, context: InferenceContext
+    ) -> nodes.ClassDef | None:  # noqa: C901
         """Try to infer what type.__new__(mcs, name, bases, attrs) returns.
 
         In order for such call to be valid, the metaclass needs to be
         a subtype of ``type``, the name needs to be a string, the bases
         needs to be a tuple of classes
         """
         # pylint: disable=import-outside-toplevel; circular import
         from astroid.nodes import Pass
 
         # Verify the metaclass
         try:
             mcs = next(caller.args[0].infer(context=context))
         except StopIteration as e:
             raise InferenceError(context=context) from e
-        if mcs.__class__.__name__ != "ClassDef":
+        if not isinstance(mcs, nodes.ClassDef):
             # Not a valid first argument.
             return None
         if not mcs.is_subtype_of("builtins.type"):
             # Not a valid metaclass.
             return None
 
         # Verify the name
         try:
             name = next(caller.args[1].infer(context=context))
         except StopIteration as e:
             raise InferenceError(context=context) from e
-        if name.__class__.__name__ != "Const":
+        if not isinstance(name, nodes.Const):
             # Not a valid name, needs to be a const.
             return None
         if not isinstance(name.value, str):
             # Needs to be a string.
             return None
 
         # Verify the bases
         try:
             bases = next(caller.args[2].infer(context=context))
         except StopIteration as e:
             raise InferenceError(context=context) from e
-        if bases.__class__.__name__ != "Tuple":
+        if not isinstance(bases, nodes.Tuple):
             # Needs to be a tuple.
             return None
         try:
             inferred_bases = [next(elt.infer(context=context)) for elt in bases.elts]
         except StopIteration as e:
             raise InferenceError(context=context) from e
-        if any(base.__class__.__name__ != "ClassDef" for base in inferred_bases):
+        if any(not isinstance(base, nodes.ClassDef) for base in inferred_bases):
             # All the bases needs to be Classes
             return None
 
         # Verify the attributes.
         try:
             attrs = next(caller.args[3].infer(context=context))
         except StopIteration as e:
             raise InferenceError(context=context) from e
-        if attrs.__class__.__name__ != "Dict":
+        if not isinstance(attrs, nodes.Dict):
             # Needs to be a dictionary.
             return None
-        cls_locals = collections.defaultdict(list)
+        cls_locals: dict[str, list[InferenceResult]] = collections.defaultdict(list)
         for key, value in attrs.items:
             try:
                 key = next(key.infer(context=context))
             except StopIteration as e:
                 raise InferenceError(context=context) from e
             try:
                 value = next(value.infer(context=context))
             except StopIteration as e:
                 raise InferenceError(context=context) from e
             # Ignore non string keys
-            if key.__class__.__name__ == "Const" and isinstance(key.value, str):
+            if isinstance(key, nodes.Const) and isinstance(key.value, str):
                 cls_locals[key.value].append(value)
 
         # Build the class from now.
         cls = mcs.__class__(
             name=name.value,
-            lineno=caller.lineno,
-            col_offset=caller.col_offset,
+            lineno=caller.lineno or 0,
+            col_offset=caller.col_offset or 0,
             parent=caller,
             end_lineno=caller.end_lineno,
             end_col_offset=caller.end_col_offset,
         )
         empty = Pass(
             parent=cls,
             lineno=caller.lineno,
             col_offset=caller.col_offset,
             end_lineno=caller.end_lineno,
             end_col_offset=caller.end_col_offset,
         )
         cls.postinit(
             bases=bases.elts,
             body=[empty],
-            decorators=[],
+            decorators=None,
             newstyle=True,
             metaclass=mcs,
             keywords=[],
         )
         cls.locals = cls_locals
         return cls
 
     def infer_call_result(
         self,
         caller: SuccessfulInferenceResult | None,
         context: InferenceContext | None = None,
     ) -> Iterator[InferenceResult]:
         context = bind_context_to_node(context, self.bound)
         if (
-            self.bound.__class__.__name__ == "ClassDef"
+            isinstance(self.bound, nodes.ClassDef)
             and self.bound.name == "type"
             and self.name == "__new__"
+            and isinstance(caller, nodes.Call)
             and len(caller.args) == 4
         ):
             # Check if we have a ``type.__new__(mcs, name, bases, attrs)`` call.
             new_cls = self._infer_type_new_call(caller, context)
             if new_cls:
                 return iter((new_cls,))
 
@@ -651,24 +679,26 @@
 
     # We defer initialization of special_attributes to the __init__ method since the constructor
     # of GeneratorModel requires the raw_building to be complete
     # TODO: This should probably be refactored.
     special_attributes: objectmodel.GeneratorModel
 
     def __init__(
-        self, parent=None, generator_initial_context: InferenceContext | None = None
-    ):
+        self,
+        parent: nodes.FunctionDef,
+        generator_initial_context: InferenceContext | None = None,
+    ) -> None:
         super().__init__()
         self.parent = parent
         self._call_context = copy_context(generator_initial_context)
 
         # See comment above: this is a deferred initialization.
         Generator.special_attributes = objectmodel.GeneratorModel()
 
-    def infer_yield_types(self):
+    def infer_yield_types(self) -> Iterator[InferenceResult]:
         yield from self.parent.infer_yield_result(self._call_context)
 
     def callable(self) -> Literal[False]:
         return False
 
     def pytype(self) -> str:
         return "builtins.generator"
```

### Comparing `astroid-3.0.0a2/astroid/brain/brain_argparse.py` & `astroid-3.0.0a3/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_attrs.py` & `astroid-3.0.0a3/astroid/brain/brain_attrs.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_boto3.py` & `astroid-3.0.0a3/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_builtin_inference.py` & `astroid-3.0.0a3/astroid/brain/brain_builtin_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Astroid hooks for various builtins."""
 
 from __future__ import annotations
 
 import itertools
-from collections.abc import Iterator
+from collections.abc import Callable, Iterable, Iterator
 from functools import partial
+from typing import Any
 
-from astroid import arguments, helpers, inference_tip, nodes, objects, util
+from astroid import arguments, bases, helpers, inference_tip, nodes, objects, util
 from astroid.builder import AstroidBuilder
 from astroid.context import InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     MroError,
     UseInferenceDefault,
 )
 from astroid.manager import AstroidManager
 from astroid.nodes import scoped_nodes
+from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
 OBJECT_DUNDER_NEW = "object.__new__"
 
 STR_CLASS = """
 class whatever(object):
     def join(self, iterable):
         return {rvalue}
@@ -191,18 +193,29 @@
     AstroidManager().register_transform(
         nodes.Call,
         inference_tip(_transform_wrapper),
         partial(_builtin_filter_predicate, builtin_name=builtin_name),
     )
 
 
-def _container_generic_inference(node, context, node_type, transform):
+def _container_generic_inference(
+    node: nodes.Call,
+    context: InferenceContext | None,
+    node_type: type[nodes.BaseContainer],
+    transform: Callable[[SuccessfulInferenceResult], nodes.BaseContainer | None],
+) -> nodes.BaseContainer:
     args = node.args
     if not args:
-        return node_type()
+        return node_type(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            parent=node.parent,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+        )
     if len(node.args) > 1:
         raise UseInferenceDefault()
 
     (arg,) = args
     transformed = transform(arg)
     if not transformed:
         try:
@@ -214,16 +227,20 @@
         transformed = transform(inferred)
     if not transformed or isinstance(transformed, util.UninferableBase):
         raise UseInferenceDefault
     return transformed
 
 
 def _container_generic_transform(  # pylint: disable=inconsistent-return-statements
-    arg, context, klass, iterables, build_elts
-):
+    arg: SuccessfulInferenceResult,
+    context: InferenceContext | None,
+    klass: type[nodes.BaseContainer],
+    iterables: tuple[type[nodes.NodeNG] | type[bases.Proxy], ...],
+    build_elts: type[Iterable[Any]],
+) -> nodes.BaseContainer | None:
     if isinstance(arg, klass):
         return arg
     if isinstance(arg, iterables):
         if all(isinstance(elt, nodes.Const) for elt in arg.elts):
             elts = [elt.value for elt in arg.elts]
         else:
             # TODO: Does not handle deduplication for sets.
@@ -246,16 +263,20 @@
         elts = arg.value
     else:
         return
     return klass.from_elements(elts=build_elts(elts))
 
 
 def _infer_builtin_container(
-    node, context, klass=None, iterables=None, build_elts=None
-):
+    node: nodes.Call,
+    context: InferenceContext | None,
+    klass: type[nodes.BaseContainer],
+    iterables: tuple[type[nodes.NodeNG] | type[bases.Proxy], ...],
+    build_elts: type[Iterable[Any]],
+) -> nodes.BaseContainer:
     transform_func = partial(
         _container_generic_transform,
         context=context,
         klass=klass,
         iterables=iterables,
         build_elts=build_elts,
     )
@@ -332,15 +353,15 @@
                 raise UseInferenceDefault()
             items.append(tuple(elt.elts))
     else:
         raise UseInferenceDefault()
     return items
 
 
-def infer_dict(node, context: InferenceContext | None = None):
+def infer_dict(node: nodes.Call, context: InferenceContext | None = None) -> nodes.Dict:
     """Try to infer a dict call to a Dict node.
 
     The function treats the following cases:
 
         * dict()
         * dict(mapping)
         * dict(iterable)
@@ -355,29 +376,39 @@
         raise UseInferenceDefault
 
     args = call.positional_arguments
     kwargs = list(call.keyword_arguments.items())
 
     if not args and not kwargs:
         # dict()
-        return nodes.Dict()
+        return nodes.Dict(
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            parent=node.parent,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+        )
     if kwargs and not args:
         # dict(a=1, b=2, c=4)
         items = [(nodes.Const(key), value) for key, value in kwargs]
     elif len(args) == 1 and kwargs:
         # dict(some_iterable, b=2, c=4)
         elts = _get_elts(args[0], context)
         keys = [(nodes.Const(key), value) for key, value in kwargs]
         items = elts + keys
     elif len(args) == 1:
         items = _get_elts(args[0], context)
     else:
         raise UseInferenceDefault()
     value = nodes.Dict(
-        col_offset=node.col_offset, lineno=node.lineno, parent=node.parent
+        col_offset=node.col_offset,
+        lineno=node.lineno,
+        parent=node.parent,
+        end_lineno=node.end_lineno,
+        end_col_offset=node.end_col_offset,
     )
     value.postinit(items)
     return value
 
 
 def infer_super(
     node: nodes.Call, context: InferenceContext | None = None
@@ -703,20 +734,20 @@
     except AstroidTypeError as exc:
         raise UseInferenceDefault("TypeError: " + str(exc)) from exc
     except MroError as exc:
         raise UseInferenceDefault from exc
     return nodes.Const(issubclass_bool)
 
 
-def infer_isinstance(callnode, context: InferenceContext | None = None):
+def infer_isinstance(
+    callnode: nodes.Call, context: InferenceContext | None = None
+) -> nodes.Const:
     """Infer isinstance calls.
 
     :param nodes.Call callnode: an isinstance call
-    :rtype nodes.Const: Boolean Const value of isinstance call
-
     :raises UseInferenceDefault: If the node cannot be inferred
     """
     call = arguments.CallSite.from_call(callnode, context=context)
     if call.keyword_arguments:
         # isinstance doesn't support keyword arguments
         raise UseInferenceDefault("TypeError: isinstance() takes no keyword arguments")
     if len(call.positional_arguments) != 2:
@@ -740,15 +771,17 @@
     except MroError as exc:
         raise UseInferenceDefault from exc
     if isinstance(isinstance_bool, util.UninferableBase):
         raise UseInferenceDefault
     return nodes.Const(isinstance_bool)
 
 
-def _class_or_tuple_to_container(node, context: InferenceContext | None = None):
+def _class_or_tuple_to_container(
+    node: InferenceResult, context: InferenceContext | None = None
+) -> list[InferenceResult]:
     # Move inferences results into container
     # to simplify later logic
     # raises InferenceError if any of the inferences fall through
     try:
         node_infer = next(node.infer(context=context))
     except StopIteration as e:
         raise InferenceError(node=node, context=context) from e
@@ -757,17 +790,14 @@
     if isinstance(node_infer, nodes.Tuple):
         try:
             class_container = [
                 next(node.infer(context=context)) for node in node_infer.elts
             ]
         except StopIteration as e:
             raise InferenceError(node=node, context=context) from e
-        class_container = [
-            klass_node for klass_node in class_container if klass_node is not None
-        ]
     else:
         class_container = [node_infer]
     return class_container
 
 
 def infer_len(node, context: InferenceContext | None = None):
     """Infer length calls.
@@ -849,15 +879,19 @@
         a Dictionary containing the values that astroid was able to infer.
         In case the inference failed for any reason, an empty dictionary
         will be inferred instead.
     """
 
     def _build_dict_with_elements(elements):
         new_node = nodes.Dict(
-            col_offset=node.col_offset, lineno=node.lineno, parent=node.parent
+            col_offset=node.col_offset,
+            lineno=node.lineno,
+            parent=node.parent,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
         )
         new_node.postinit(elements)
         return new_node
 
     call = arguments.CallSite.from_call(node, context=context)
     if call.keyword_arguments:
         raise UseInferenceDefault("TypeError: int() must take no keyword arguments")
```

### Comparing `astroid-3.0.0a2/astroid/brain/brain_collections.py` & `astroid-3.0.0a3/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_crypt.py` & `astroid-3.0.0a3/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_ctypes.py` & `astroid-3.0.0a3/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_curses.py` & `astroid-3.0.0a3/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_dataclasses.py` & `astroid-3.0.0a3/astroid/brain/brain_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_dateutil.py` & `astroid-3.0.0a3/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_fstrings.py` & `astroid-3.0.0a3/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_functools.py` & `astroid-3.0.0a3/astroid/brain/brain_functools.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_gi.py` & `astroid-3.0.0a3/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_hashlib.py` & `astroid-3.0.0a3/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_http.py` & `astroid-3.0.0a3/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_hypothesis.py` & `astroid-3.0.0a3/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_io.py` & `astroid-3.0.0a3/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_mechanize.py` & `astroid-3.0.0a3/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_multiprocessing.py` & `astroid-3.0.0a3/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.0.0a3/astroid/brain/brain_namedtuple_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,15 +219,17 @@
     call_site = arguments.CallSite.from_call(node, context=context)
     node = extract_node("import collections; collections.namedtuple")
     try:
         func = next(node.infer())
     except StopIteration as e:
         raise InferenceError(node=node) from e
     try:
-        rename = next(call_site.infer_argument(func, "rename", context)).bool_value()
+        rename = next(
+            call_site.infer_argument(func, "rename", context or InferenceContext())
+        ).bool_value()
     except (InferenceError, StopIteration):
         rename = False
 
     try:
         attributes = _check_namedtuple_attributes(name, attributes, rename)
     except AstroidTypeError as exc:
         raise UseInferenceDefault("TypeError: " + str(exc)) from exc
@@ -460,17 +462,31 @@
                 for method in node.mymethods():
                     fake.locals[method.name] = [method]
                 new_targets.append(fake.instantiate_class())
                 dunder_members[local] = fake
             node.locals[local] = new_targets
 
         # The undocumented `_value2member_map_` member:
-        node.locals["_value2member_map_"] = [nodes.Dict(parent=node)]
+        node.locals["_value2member_map_"] = [
+            nodes.Dict(
+                parent=node,
+                lineno=node.lineno,
+                col_offset=node.col_offset,
+                end_lineno=node.end_lineno,
+                end_col_offset=node.end_col_offset,
+            )
+        ]
 
-        members = nodes.Dict(parent=node)
+        members = nodes.Dict(
+            parent=node,
+            lineno=node.lineno,
+            col_offset=node.col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
+        )
         members.postinit(
             [
                 (
                     nodes.Const(k, parent=members),
                     nodes.Name(
                         v.name,
                         parent=members,
```

### Comparing `astroid-3.0.0a2/astroid/brain/brain_nose.py` & `astroid-3.0.0a3/astroid/brain/brain_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_core_einsumfunc.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_ma.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_numpy_utils.py` & `astroid-3.0.0a3/astroid/brain/brain_numpy_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_pathlib.py` & `astroid-3.0.0a3/astroid/brain/brain_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_pkg_resources.py` & `astroid-3.0.0a3/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_pytest.py` & `astroid-3.0.0a3/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_qt.py` & `astroid-3.0.0a3/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_random.py` & `astroid-3.0.0a3/astroid/brain/brain_random.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_re.py` & `astroid-3.0.0a3/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_regex.py` & `astroid-3.0.0a3/astroid/brain/brain_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_responses.py` & `astroid-3.0.0a3/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_scipy_signal.py` & `astroid-3.0.0a3/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_signal.py` & `astroid-3.0.0a3/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_six.py` & `astroid-3.0.0a3/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_sqlalchemy.py` & `astroid-3.0.0a3/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_ssl.py` & `astroid-3.0.0a3/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_subprocess.py` & `astroid-3.0.0a3/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_threading.py` & `astroid-3.0.0a3/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_type.py` & `astroid-3.0.0a3/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_typing.py` & `astroid-3.0.0a3/astroid/brain/brain_typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_unittest.py` & `astroid-3.0.0a3/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/brain_uuid.py` & `astroid-3.0.0a3/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/brain/helpers.py` & `astroid-3.0.0a3/astroid/brain/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/builder.py` & `astroid-3.0.0a3/astroid/builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/const.py` & `astroid-3.0.0a3/astroid/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/constraint.py` & `astroid-3.0.0a3/astroid/constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/context.py` & `astroid-3.0.0a3/astroid/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 """Various context related utilities, including inference and call contexts."""
 
 from __future__ import annotations
 
 import contextlib
 import pprint
+from collections.abc import Iterator
 from typing import TYPE_CHECKING, Dict, Optional, Sequence, Tuple
 
-from astroid.typing import InferenceResult
+from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
 if TYPE_CHECKING:
     from astroid import constraint, nodes
     from astroid.nodes.node_classes import Keyword, NodeNG
 
 _InferenceCache = Dict[
     Tuple["NodeNG", Optional[str], Optional[str], Optional[str]], Sequence["NodeNG"]
@@ -44,54 +45,43 @@
         "_nodes_inferred",
     )
 
     max_inferred = 100
 
     def __init__(
         self,
-        path=None,
+        path: set[tuple[nodes.NodeNG, str | None]] | None = None,
         nodes_inferred: list[int] | None = None,
-    ):
+    ) -> None:
         if nodes_inferred is None:
             self._nodes_inferred = [0]
         else:
             self._nodes_inferred = nodes_inferred
 
         self.path = path or set()
-        """
-        :type: set(tuple(NodeNG, optional(str)))
-
-        Path of visited nodes and their lookupname
+        """Path of visited nodes and their lookupname.
 
         Currently this key is ``(node, context.lookupname)``
         """
         self.lookupname: str | None = None
         """The original name of the node.
 
         e.g.
         foo = 1
         The inference of 'foo' is nodes.Const(1) but the lookup name is 'foo'
         """
         self.callcontext: CallContext | None = None
         """The call arguments and keywords for the given context."""
-        self.boundnode = None
-        """
-        :type: optional[NodeNG]
-
-        The bound node of the given context
+        self.boundnode: SuccessfulInferenceResult | None = None
+        """The bound node of the given context.
 
         e.g. the bound node of object.__new__(cls) is the object node
         """
-        self.extra_context = {}
-        """
-        :type: dict(NodeNG, Context)
-
-        Context that needs to be passed down through call stacks
-        for call arguments
-        """
+        self.extra_context: dict[SuccessfulInferenceResult, InferenceContext] = {}
+        """Context that needs to be passed down through call stacks for call arguments."""
 
         self.constraints: dict[str, dict[nodes.If, set[constraint.Constraint]]] = {}
         """The constraints on nodes."""
 
     @property
     def nodes_inferred(self) -> int:
         """
@@ -112,19 +102,17 @@
         Inferred node contexts to their mapped results.
 
         Currently the key is ``(node, lookupname, callcontext, boundnode)``
         and the value is tuple of the inferred results
         """
         return _INFERENCE_CACHE
 
-    def push(self, node) -> bool:
+    def push(self, node: nodes.NodeNG) -> bool:
         """Push node into inference path.
 
-        :return: Whether node is already in context path.
-
         Allows one to see if the given node has already
         been looked at for this inference context
         """
         name = self.lookupname
         if (node, name) in self.path:
             return True
 
@@ -143,15 +131,15 @@
         clone.callcontext = self.callcontext
         clone.boundnode = self.boundnode
         clone.extra_context = self.extra_context
         clone.constraints = self.constraints.copy()
         return clone
 
     @contextlib.contextmanager
-    def restore_path(self):
+    def restore_path(self) -> Iterator[None]:
         path = set(self.path)
         yield
         self.path = path
 
     def __str__(self) -> str:
         state = (
             f"{field}={pprint.pformat(getattr(self, field), width=80 - len(field))}"
@@ -184,24 +172,20 @@
     """Clone a context if given, or return a fresh context."""
     if context is not None:
         return context.clone()
 
     return InferenceContext()
 
 
-def bind_context_to_node(context: InferenceContext | None, node) -> InferenceContext:
+def bind_context_to_node(
+    context: InferenceContext | None, node: SuccessfulInferenceResult
+) -> InferenceContext:
     """Give a context a boundnode
     to retrieve the correct function name or attribute value
     with from further inference.
 
     Do not use an existing context since the boundnode could then
     be incorrectly propagated higher up in the call stack.
-
-    :param node: Node to do name lookups from
-    :type node NodeNG:
-
-    :returns: A new context
-    :rtype: InferenceContext
     """
     context = copy_context(context)
     context.boundnode = node
     return context
```

### Comparing `astroid-3.0.0a2/astroid/decorators.py` & `astroid-3.0.0a3/astroid/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     ) -> Generator[InferenceResult, None, None]:
         generator = func(*args, **kwargs)
         try:
             yield next(generator)
         except StopIteration as error:
             # generator is empty
             if error.args:
-                # pylint: disable=not-a-mapping
                 raise InferenceError(**error.args[0]) from error
             raise InferenceError(
                 "StopIteration raised without any error information."
             ) from error
         except RecursionError as error:
             raise InferenceError(
                 f"RecursionError raised with limit {sys.getrecursionlimit()}."
```

### Comparing `astroid-3.0.0a2/astroid/exceptions.py` & `astroid-3.0.0a3/astroid/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """This module contains exceptions used in the astroid library."""
 
 from __future__ import annotations
 
-from collections.abc import Sequence
+from collections.abc import Iterator
 from typing import TYPE_CHECKING, Any
 
 from astroid import util
-from astroid.typing import InferenceResult
+from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
 if TYPE_CHECKING:
     from astroid import arguments, bases, nodes, objects
     from astroid.context import InferenceContext
 
 __all__ = (
     "AstroidBuildingError",
@@ -241,19 +241,19 @@
         node: InferenceResult | None = None,
         context: InferenceContext | None = None,
         target: InferenceResult | None = None,
         targets: InferenceResult | None = None,
         attribute: str | None = None,
         unknown: InferenceResult | None = None,
         assign_path: list[int] | None = None,
-        caller: nodes.Call | None = None,
-        stmts: Sequence[InferenceResult] | None = None,
+        caller: SuccessfulInferenceResult | None = None,
+        stmts: Iterator[InferenceResult] | None = None,
         frame: InferenceResult | None = None,
         call_site: arguments.CallSite | None = None,
-        func: nodes.FunctionDef | None = None,
+        func: InferenceResult | None = None,
         arg: str | None = None,
         positional_arguments: list | None = None,
         unpacked_args: list | None = None,
         keyword_arguments: dict | None = None,
         unpacked_kwargs: dict | None = None,
         **kws: Any,
     ) -> None:
```

### Comparing `astroid-3.0.0a2/astroid/filter_statements.py` & `astroid-3.0.0a3/astroid/filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/helpers.py` & `astroid-3.0.0a3/astroid/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,50 +4,51 @@
 
 """Various helper utilities."""
 
 from __future__ import annotations
 
 from collections.abc import Generator
 
-from astroid import bases, manager, nodes, raw_building, util
+from astroid import bases, manager, nodes, objects, raw_building, util
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
     MroError,
     _NonDeducibleTypeHierarchy,
 )
 from astroid.nodes import scoped_nodes
-from astroid.typing import InferenceResult, SuccessfulInferenceResult
+from astroid.typing import InferenceResult
 
 
 def _build_proxy_class(cls_name: str, builtins: nodes.Module) -> nodes.ClassDef:
     proxy = raw_building.build_class(cls_name)
     proxy.parent = builtins
     return proxy
 
 
 def _function_type(
-    function: nodes.Lambda | bases.UnboundMethod, builtins: nodes.Module
+    function: nodes.Lambda | nodes.FunctionDef | bases.UnboundMethod,
+    builtins: nodes.Module,
 ) -> nodes.ClassDef:
     if isinstance(function, (scoped_nodes.Lambda, scoped_nodes.FunctionDef)):
         if function.root().name == "builtins":
             cls_name = "builtin_function_or_method"
         else:
             cls_name = "function"
     elif isinstance(function, bases.BoundMethod):
         cls_name = "method"
     else:
         cls_name = "function"
     return _build_proxy_class(cls_name, builtins)
 
 
 def _object_type(
-    node: SuccessfulInferenceResult, context: InferenceContext | None = None
+    node: InferenceResult, context: InferenceContext | None = None
 ) -> Generator[InferenceResult | None, None, None]:
     astroid_manager = manager.AstroidManager()
     builtins = astroid_manager.builtins_module
     context = context or InferenceContext()
 
     for inferred in node.infer(context=context):
         if isinstance(inferred, scoped_nodes.ClassDef):
@@ -64,22 +65,22 @@
             yield _function_type(inferred, builtins)
         elif isinstance(inferred, scoped_nodes.Module):
             yield _build_proxy_class("module", builtins)
         elif isinstance(inferred, nodes.Unknown):
             raise InferenceError
         elif isinstance(inferred, util.UninferableBase):
             yield inferred
-        elif isinstance(inferred, (bases.Proxy, nodes.Slice)):
+        elif isinstance(inferred, (bases.Proxy, nodes.Slice, objects.Super)):
             yield inferred._proxied
         else:  # pragma: no cover
             raise AssertionError(f"We don't handle {type(inferred)} currently")
 
 
 def object_type(
-    node: SuccessfulInferenceResult, context: InferenceContext | None = None
+    node: InferenceResult, context: InferenceContext | None = None
 ) -> InferenceResult | None:
     """Obtain the type of the given node.
 
     This is used to implement the ``type`` builtin, which means that it's
     used for inferring type calls, as well as used in a couple of other places
     in the inference.
     The node will be inferred first, so this function can support all
@@ -92,81 +93,83 @@
         return util.Uninferable
     if len(types) > 1 or not types:
         return util.Uninferable
     return list(types)[0]
 
 
 def _object_type_is_subclass(
-    obj_type, class_or_seq, context: InferenceContext | None = None
-):
-    if not isinstance(class_or_seq, (tuple, list)):
-        class_seq = (class_or_seq,)
-    else:
-        class_seq = class_or_seq
-
-    if isinstance(obj_type, util.UninferableBase):
+    obj_type: InferenceResult | None,
+    class_or_seq: list[InferenceResult],
+    context: InferenceContext | None = None,
+) -> util.UninferableBase | bool:
+    if isinstance(obj_type, util.UninferableBase) or not isinstance(
+        obj_type, nodes.ClassDef
+    ):
         return util.Uninferable
 
     # Instances are not types
     class_seq = [
         item if not isinstance(item, bases.Instance) else util.Uninferable
-        for item in class_seq
+        for item in class_or_seq
     ]
     # strict compatibility with issubclass
     # issubclass(type, (object, 1)) evaluates to true
     # issubclass(object, (1, type)) raises TypeError
     for klass in class_seq:
         if isinstance(klass, util.UninferableBase):
             raise AstroidTypeError("arg 2 must be a type or tuple of types")
 
         for obj_subclass in obj_type.mro():
             if obj_subclass == klass:
                 return True
     return False
 
 
-def object_isinstance(node, class_or_seq, context: InferenceContext | None = None):
+def object_isinstance(
+    node: InferenceResult,
+    class_or_seq: list[InferenceResult],
+    context: InferenceContext | None = None,
+) -> util.UninferableBase | bool:
     """Check if a node 'isinstance' any node in class_or_seq.
 
-    :param node: A given node
-    :param class_or_seq: Union[nodes.NodeNG, Sequence[nodes.NodeNG]]
-    :rtype: bool
-
     :raises AstroidTypeError: if the given ``classes_or_seq`` are not types
     """
     obj_type = object_type(node, context)
     if isinstance(obj_type, util.UninferableBase):
         return util.Uninferable
     return _object_type_is_subclass(obj_type, class_or_seq, context=context)
 
 
-def object_issubclass(node, class_or_seq, context: InferenceContext | None = None):
+def object_issubclass(
+    node: nodes.NodeNG,
+    class_or_seq: list[InferenceResult],
+    context: InferenceContext | None = None,
+) -> util.UninferableBase | bool:
     """Check if a type is a subclass of any node in class_or_seq.
 
-    :param node: A given node
-    :param class_or_seq: Union[Nodes.NodeNG, Sequence[nodes.NodeNG]]
-    :rtype: bool
-
     :raises AstroidTypeError: if the given ``classes_or_seq`` are not types
     :raises AstroidError: if the type of the given node cannot be inferred
         or its type's mro doesn't work
     """
     if not isinstance(node, nodes.ClassDef):
         raise TypeError(f"{node} needs to be a ClassDef node")
     return _object_type_is_subclass(node, class_or_seq, context=context)
 
 
 def safe_infer(
-    node: nodes.NodeNG | bases.Proxy, context: InferenceContext | None = None
+    node: nodes.NodeNG | bases.Proxy | util.UninferableBase,
+    context: InferenceContext | None = None,
 ) -> InferenceResult | None:
     """Return the inferred value for the given node.
 
     Return None if inference failed or if there is some ambiguity (more than
     one node has been inferred).
     """
+    if isinstance(node, util.UninferableBase):
+        return node
     try:
         inferit = node.infer(context=context)
         value = next(inferit)
     except (InferenceError, StopIteration):
         return None
     try:
         next(inferit)
@@ -263,15 +266,15 @@
 
     # prevent self referential length calls from causing a recursion error
     # see https://github.com/pylint-dev/astroid/issues/777
     node_frame = node.frame(future=True)
     if (
         isinstance(node_frame, scoped_nodes.FunctionDef)
         and node_frame.name == "__len__"
-        and hasattr(inferred_node, "_proxied")
+        and isinstance(inferred_node, bases.Proxy)
         and inferred_node._proxied == node_frame.parent
     ):
         message = (
             "Self referential __len__ function will "
             "cause a RecursionError on line {} of {}".format(
                 node.lineno, node.root().file
             )
```

### Comparing `astroid-3.0.0a2/astroid/inference.py` & `astroid-3.0.0a3/astroid/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,19 @@
 ) -> Iterator[_BaseContainerT]:
     has_starred_named_expr = any(
         isinstance(e, (nodes.Starred, nodes.NamedExpr)) for e in self.elts
     )
     if has_starred_named_expr:
         values = _infer_sequence_helper(self, context)
         new_seq = type(self)(
-            lineno=self.lineno, col_offset=self.col_offset, parent=self.parent
+            lineno=self.lineno,
+            col_offset=self.col_offset,
+            parent=self.parent,
+            end_lineno=self.end_lineno,
+            end_col_offset=self.end_col_offset,
         )
         new_seq.postinit(values)
 
         yield new_seq
     else:
         yield self
 
@@ -147,15 +151,21 @@
 def infer_map(
     self: nodes.Dict, context: InferenceContext | None = None
 ) -> Iterator[nodes.Dict]:
     if not any(isinstance(k, nodes.DictUnpack) for k, _ in self.items):
         yield self
     else:
         items = _infer_map(self, context)
-        new_seq = type(self)(self.lineno, self.col_offset, self.parent)
+        new_seq = type(self)(
+            self.lineno,
+            self.col_offset,
+            self.parent,
+            end_lineno=self.end_lineno,
+            end_col_offset=self.end_col_offset,
+        )
         new_seq.postinit(list(items.items()))
         yield new_seq
 
 
 def _update_with_replacement(
     lhs_dict: dict[SuccessfulInferenceResult, SuccessfulInferenceResult],
     rhs_dict: dict[SuccessfulInferenceResult, SuccessfulInferenceResult],
@@ -250,15 +260,14 @@
     context = copy_context(context)
     context.lookupname = self.name
     context.constraints[self.name] = constraint.get_constraints(self, frame)
 
     return bases._infer_stmts(stmts, context, frame)
 
 
-# pylint: disable=no-value-for-parameter
 # The order of the decorators here is important
 # See https://github.com/pylint-dev/astroid/commit/0a8a75db30da060a24922e05048bc270230f5
 nodes.Name._infer = decorators.raise_if_nothing_inferred(
     decorators.path_wrapper(infer_name)
 )
 nodes.AssignName.infer_lhs = infer_name  # won't work with a path wrapper
 
@@ -1005,23 +1014,23 @@
 }
 UNINFERABLE_OPS = {
     "is",
     "is not",
 }
 
 
-def _to_literal(node: nodes.NodeNG) -> Any:
+def _to_literal(node: SuccessfulInferenceResult) -> Any:
     # Can raise SyntaxError or ValueError from ast.literal_eval
     # Can raise AttributeError from node.as_string() as not all nodes have a visitor
     # Is this the stupidest idea or the simplest idea?
     return ast.literal_eval(node.as_string())
 
 
 def _do_compare(
-    left_iter: Iterable[nodes.NodeNG], op: str, right_iter: Iterable[nodes.NodeNG]
+    left_iter: Iterable[InferenceResult], op: str, right_iter: Iterable[InferenceResult]
 ) -> bool | util.UninferableBase:
     """
     If all possible combinations are either True or False, return that:
     >>> _do_compare([1, 2], '<=', [3, 4])
     True
     >>> _do_compare([1, 2], '==', [3, 4])
     False
```

### Comparing `astroid-3.0.0a2/astroid/inference_tip.py` & `astroid-3.0.0a3/astroid/inference_tip.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,55 +2,75 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Transform utilities (filters and decorator)."""
 
 from __future__ import annotations
 
-from collections.abc import Callable, Iterator
-
-from typing_extensions import ParamSpec
+from collections.abc import Generator
+from typing import Any, TypeVar
 
+from astroid.context import InferenceContext
 from astroid.exceptions import InferenceOverwriteError, UseInferenceDefault
 from astroid.nodes import NodeNG
-from astroid.typing import InferenceResult, InferFn
+from astroid.typing import (
+    InferenceResult,
+    InferFn,
+    TransformFn,
+)
+
+_cache: dict[
+    tuple[InferFn[Any], NodeNG, InferenceContext | None], list[InferenceResult]
+] = {}
 
-_P = ParamSpec("_P")
+_CURRENTLY_INFERRING: set[tuple[InferFn[Any], NodeNG]] = set()
 
-_cache: dict[tuple[InferFn, NodeNG], list[InferenceResult] | None] = {}
+_NodesT = TypeVar("_NodesT", bound=NodeNG)
 
 
 def clear_inference_tip_cache() -> None:
     """Clear the inference tips cache."""
     _cache.clear()
 
 
-def _inference_tip_cached(
-    func: Callable[_P, Iterator[InferenceResult]],
-) -> Callable[_P, Iterator[InferenceResult]]:
+def _inference_tip_cached(func: InferFn[_NodesT]) -> InferFn[_NodesT]:
     """Cache decorator used for inference tips."""
 
-    def inner(*args: _P.args, **kwargs: _P.kwargs) -> Iterator[InferenceResult]:
-        node = args[0]
-        try:
-            result = _cache[func, node]
+    def inner(
+        node: _NodesT,
+        context: InferenceContext | None = None,
+        **kwargs: Any,
+    ) -> Generator[InferenceResult, None, None]:
+        partial_cache_key = (func, node)
+        if partial_cache_key in _CURRENTLY_INFERRING:
             # If through recursion we end up trying to infer the same
             # func + node we raise here.
-            if result is None:
-                raise UseInferenceDefault()
+            raise UseInferenceDefault
+        try:
+            yield from _cache[func, node, context]
+            return
         except KeyError:
-            _cache[func, node] = None
-            result = _cache[func, node] = list(func(*args, **kwargs))
-            assert result
-        return iter(result)
+            # Recursion guard with a partial cache key.
+            # Using the full key causes a recursion error on PyPy.
+            # It's a pragmatic compromise to avoid so much recursive inference
+            # with slightly different contexts while still passing the simple
+            # test cases included with this commit.
+            _CURRENTLY_INFERRING.add(partial_cache_key)
+            result = _cache[func, node, context] = list(func(node, context, **kwargs))
+            # Remove recursion guard.
+            _CURRENTLY_INFERRING.remove(partial_cache_key)
+
+        yield from result
 
     return inner
 
 
-def inference_tip(infer_function: InferFn, raise_on_overwrite: bool = False) -> InferFn:
+def inference_tip(
+    infer_function: InferFn[_NodesT], raise_on_overwrite: bool = False
+) -> TransformFn[_NodesT]:
     """Given an instance specific inference function, return a function to be
     given to AstroidManager().register_transform to set this inference function.
 
     :param bool raise_on_overwrite: Raise an `InferenceOverwriteError`
         if the inference tip will overwrite another. Used for debugging
 
     Typical usage
@@ -64,26 +84,27 @@
 
         Using an inference tip will override
         any previously set inference tip for the given
         node. Use a predicate in the transform to prevent
         excess overwrites.
     """
 
-    def transform(node: NodeNG, infer_function: InferFn = infer_function) -> NodeNG:
+    def transform(
+        node: _NodesT, infer_function: InferFn[_NodesT] = infer_function
+    ) -> _NodesT:
         if (
             raise_on_overwrite
             and node._explicit_inference is not None
             and node._explicit_inference is not infer_function
         ):
             raise InferenceOverwriteError(
                 "Inference already set to {existing_inference}. "
                 "Trying to overwrite with {new_inference} for {node}".format(
                     existing_inference=infer_function,
                     new_inference=node._explicit_inference,
                     node=node,
                 )
             )
-        # pylint: disable=no-value-for-parameter
         node._explicit_inference = _inference_tip_cached(infer_function)
         return node
 
     return transform
```

### Comparing `astroid-3.0.0a2/astroid/interpreter/_import/spec.py` & `astroid-3.0.0a3/astroid/interpreter/_import/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         # See if we support the customer import hook of the meta_finder
         meta_finder_name = meta_finder.__class__.__name__
         if meta_finder_name not in _MetaPathFinderModuleTypes:
             # Setuptools>62 creates its EditableFinders dynamically and have
             # "type" as their __class__.__name__. We check __name__ as well
             # to see if we can support the finder.
             try:
-                meta_finder_name = meta_finder.__name__
+                meta_finder_name = meta_finder.__name__  # type: ignore[attr-defined]
             except AttributeError:
                 continue
             if meta_finder_name not in _MetaPathFinderModuleTypes:
                 continue
 
         module_type = _MetaPathFinderModuleTypes[meta_finder_name]
 
@@ -457,14 +457,15 @@
         )
         processed.append(modname)
         if modpath:
             if isinstance(finder, Finder):
                 submodule_path = finder.contribute_to_path(spec, processed)
             # If modname is a package from an editable install, update submodule_path
             # so that the next module in the path will be found inside of it using importlib.
-            elif finder.__name__ in _EditableFinderClasses:
+            # Existence of __name__ is guaranteed by _find_spec_with_path.
+            elif finder.__name__ in _EditableFinderClasses:  # type: ignore[attr-defined]
                 submodule_path = spec.submodule_search_locations
 
         if spec.type == ModuleType.PKG_DIRECTORY:
             spec = spec._replace(submodule_search_locations=submodule_path)
 
     return spec
```

### Comparing `astroid-3.0.0a2/astroid/interpreter/_import/util.py` & `astroid-3.0.0a3/astroid/interpreter/_import/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/interpreter/dunder_lookup.py` & `astroid-3.0.0a3/astroid/interpreter/dunder_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/interpreter/objectmodel.py` & `astroid-3.0.0a3/astroid/interpreter/objectmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,21 @@
     from astroid.objects import Property
 
 IMPL_PREFIX = "attr_"
 LEN_OF_IMPL_PREFIX = len(IMPL_PREFIX)
 
 
 def _dunder_dict(instance, attributes):
-    obj = node_classes.Dict(parent=instance)
+    obj = node_classes.Dict(
+        parent=instance,
+        lineno=instance.lineno,
+        col_offset=instance.col_offset,
+        end_lineno=instance.end_lineno,
+        end_col_offset=instance.end_col_offset,
+    )
 
     # Convert the keys to node strings
     keys = [
         node_classes.Const(value=value, parent=obj) for value in list(attributes.keys())
     ]
 
     # The original attribute has a list of elements for each key,
@@ -259,15 +265,21 @@
 
         defaults_obj = node_classes.Tuple(parent=func)
         defaults_obj.postinit(func.args.defaults)
         return defaults_obj
 
     @property
     def attr___annotations__(self):
-        obj = node_classes.Dict(parent=self._instance)
+        obj = node_classes.Dict(
+            parent=self._instance,
+            lineno=self._instance.lineno,
+            col_offset=self._instance.col_offset,
+            end_lineno=self._instance.end_lineno,
+            end_col_offset=self._instance.end_col_offset,
+        )
 
         if not self._instance.returns:
             returns = None
         else:
             returns = self._instance.returns
 
         args = self._instance.args
@@ -293,15 +305,21 @@
         ]
 
         obj.postinit(items)
         return obj
 
     @property
     def attr___dict__(self):
-        return node_classes.Dict(parent=self._instance)
+        return node_classes.Dict(
+            parent=self._instance,
+            lineno=self._instance.lineno,
+            col_offset=self._instance.col_offset,
+            end_lineno=self._instance.end_lineno,
+            end_col_offset=self._instance.end_col_offset,
+        )
 
     attr___globals__ = attr___dict__
 
     @property
     def attr___kwdefaults__(self):
         def _default_args(args, parent):
             for arg in args.kwonlyargs:
@@ -310,15 +328,21 @@
                 except NoDefault:
                     continue
 
                 name = node_classes.Const(arg.name, parent=parent)
                 yield name, default
 
         args = self._instance.args
-        obj = node_classes.Dict(parent=self._instance)
+        obj = node_classes.Dict(
+            parent=self._instance,
+            lineno=self._instance.lineno,
+            col_offset=self._instance.col_offset,
+            end_lineno=self._instance.end_lineno,
+            end_col_offset=self._instance.end_col_offset,
+        )
         defaults = dict(_default_args(args, obj))
 
         obj.postinit(list(defaults.items()))
         return obj
 
     @property
     def attr___module__(self):
@@ -563,15 +587,21 @@
 
         implicit_metaclass = self._instance.implicit_metaclass()
         subclasses_method = implicit_metaclass.locals["__subclasses__"][0]
         return SubclassesBoundMethod(proxy=subclasses_method, bound=implicit_metaclass)
 
     @property
     def attr___dict__(self):
-        return node_classes.Dict(parent=self._instance)
+        return node_classes.Dict(
+            parent=self._instance,
+            lineno=self._instance.lineno,
+            col_offset=self._instance.col_offset,
+            end_lineno=self._instance.end_lineno,
+            end_col_offset=self._instance.end_col_offset,
+        )
 
     @property
     def attr___call__(self):
         """Calling a class A() returns an instance of A."""
         return self._instance.instantiate_class()
```

### Comparing `astroid-3.0.0a2/astroid/manager.py` & `astroid-3.0.0a3/astroid/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,14 @@
         builder = AstroidBuilder(self)
         for ext in ZIP_IMPORT_EXTS:
             try:
                 eggpath, resource = filepath.rsplit(ext + os.path.sep, 1)
             except ValueError:
                 continue
             try:
-                # pylint: disable-next=no-member
                 importer = zipimport.zipimporter(eggpath + ext)
                 zmodname = resource.replace(os.path.sep, ".")
                 if importer.is_package(resource):
                     zmodname = zmodname + ".__init__"
                 module = builder.string_build(
                     importer.get_source(resource), zmodname, filepath
                 )
```

### Comparing `astroid-3.0.0a2/astroid/mixins.py` & `astroid-3.0.0a3/astroid/mixins.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/modutils.py` & `astroid-3.0.0a3/astroid/modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/node_classes.py` & `astroid-3.0.0a3/astroid/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/nodes/__init__.py` & `astroid-3.0.0a3/astroid/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/nodes/_base_nodes.py` & `astroid-3.0.0a3/astroid/nodes/_base_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/nodes/as_string.py` & `astroid-3.0.0a3/astroid/nodes/as_string.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/nodes/const.py` & `astroid-3.0.0a3/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/nodes/node_classes.py` & `astroid-3.0.0a3/astroid/nodes/node_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 """Module for some node classes. More nodes in scoped_nodes.py"""
 
 from __future__ import annotations
 
 import abc
 import itertools
+import sys
 import typing
 from collections.abc import Generator, Iterable, Iterator, Mapping
 from functools import cached_property, lru_cache
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -42,14 +43,20 @@
     ConstFactoryResult,
     InferBinaryOp,
     InferenceErrorInfo,
     InferenceResult,
     SuccessfulInferenceResult,
 )
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
+
 if TYPE_CHECKING:
     from astroid import nodes
     from astroid.nodes import LocalsDictNodeNG
 
 
 def _is_const(value) -> bool:
     return isinstance(value, tuple(CONST_CLS))
@@ -262,67 +269,51 @@
 class BaseContainer(_base_nodes.ParentAssignNode, Instance, metaclass=abc.ABCMeta):
     """Base class for Set, FrozenSet, Tuple and List."""
 
     _astroid_fields = ("elts",)
 
     def __init__(
         self,
-        lineno: int | None = None,
-        col_offset: int | None = None,
-        parent: NodeNG | None = None,
+        lineno: int | None,
+        col_offset: int | None,
+        parent: NodeNG | None,
         *,
-        end_lineno: int | None = None,
-        end_col_offset: int | None = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.elts: list[NodeNG] = []
+        self.elts: list[SuccessfulInferenceResult] = []
         """The elements in the node."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
-    def postinit(self, elts: list[NodeNG]) -> None:
-        """Do some setup after initialisation.
-
-        :param elts: The list of elements the that node contains.
-        """
+    def postinit(self, elts: list[SuccessfulInferenceResult]) -> None:
         self.elts = elts
 
     @classmethod
-    def from_elements(cls, elts=None):
+    def from_elements(cls, elts: Iterable[Any]) -> Self:
         """Create a node of this type from the given list of elements.
 
         :param elts: The list of elements that the node should contain.
-        :type elts: list(NodeNG)
 
         :returns: A new node containing the given elements.
-        :rtype: NodeNG
         """
-        node = cls()
-        if elts is None:
-            node.elts = []
-        else:
-            node.elts = [const_factory(e) if _is_const(e) else e for e in elts]
+        node = cls(
+            lineno=None,
+            col_offset=None,
+            parent=None,
+            end_lineno=None,
+            end_col_offset=None,
+        )
+        node.elts = [const_factory(e) if _is_const(e) else e for e in elts]
         return node
 
     def itered(self):
         """An iterator over the elements this node contains.
 
         :returns: The contents of this node.
         :rtype: iterable(NodeNG)
@@ -1851,37 +1842,22 @@
     <Dict.dict l.1 at 0x7f23b2e35cc0>
     """
 
     _astroid_fields = ("items",)
 
     def __init__(
         self,
-        lineno: int | None = None,
-        col_offset: int | None = None,
-        parent: NodeNG | None = None,
+        lineno: int | None,
+        col_offset: int | None,
+        parent: NodeNG | None,
         *,
-        end_lineno: int | None = None,
-        end_col_offset: int | None = None,
+        end_lineno: int | None,
+        end_col_offset: int | None,
     ) -> None:
-        """
-        :param lineno: The line that this node appears on in the source code.
-
-        :param col_offset: The column that this node appears on in the
-            source code.
-
-        :param parent: The parent node in the syntax tree.
-
-        :param end_lineno: The last line this node appears on in the source code.
-
-        :param end_col_offset: The end column this node appears on in the
-            source code. Note: This is after the last symbol.
-        """
-        self.items: list[
-            tuple[SuccessfulInferenceResult, SuccessfulInferenceResult]
-        ] = []
+        self.items: list[tuple[InferenceResult, InferenceResult]] = []
         """The key-value pairs contained in the dictionary."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
@@ -1895,36 +1871,14 @@
 
         :param items: The key-value pairs contained in the dictionary.
         """
         self.items = items
 
     infer_unary_op: ClassVar[InferUnaryOp[Dict]]
 
-    @classmethod
-    def from_elements(cls, items=None):
-        """Create a :class:`Dict` of constants from a live dictionary.
-
-        :param items: The items to store in the node.
-        :type items: dict
-
-        :returns: The created dictionary node.
-        :rtype: Dict
-        """
-        node = cls()
-        if items is None:
-            node.items = []
-        else:
-            node.items = [
-                (const_factory(k), const_factory(v) if _is_const(v) else v)
-                for k, v in items.items()
-                # The keys need to be constants
-                if _is_const(k)
-            ]
-        return node
-
     def pytype(self) -> Literal["builtins.dict"]:
         """Get the name of the type that this node represents.
 
         :returns: The name of the type.
         """
         return "builtins.dict"
 
@@ -4526,15 +4480,27 @@
         node = EmptyNode()
         node.object = value
         return node
 
     instance: List | Set | Tuple | Dict
     initializer_cls = CONST_CLS[value.__class__]
     if issubclass(initializer_cls, (List, Set, Tuple)):
-        instance = initializer_cls()
+        instance = initializer_cls(
+            lineno=None,
+            col_offset=None,
+            parent=None,
+            end_lineno=None,
+            end_col_offset=None,
+        )
         instance.postinit(_create_basic_elements(value, instance))
         return instance
     if issubclass(initializer_cls, Dict):
-        instance = initializer_cls()
+        instance = initializer_cls(
+            lineno=None,
+            col_offset=None,
+            parent=None,
+            end_lineno=None,
+            end_col_offset=None,
+        )
         instance.postinit(_create_dict_items(value, instance))
         return instance
     return Const(value)
```

### Comparing `astroid-3.0.0a2/astroid/nodes/node_ng.py` & `astroid-3.0.0a3/astroid/nodes/node_ng.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 from __future__ import annotations
 
 import pprint
+import sys
 import warnings
 from collections.abc import Generator, Iterator
 from functools import cached_property
 from functools import singledispatch as _singledispatch
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -33,14 +34,20 @@
 )
 from astroid.manager import AstroidManager
 from astroid.nodes.as_string import AsStringVisitor
 from astroid.nodes.const import OP_PRECEDENCE
 from astroid.nodes.utils import Position
 from astroid.typing import InferenceErrorInfo, InferenceResult, InferFn
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
+
 if TYPE_CHECKING:
     from astroid import nodes
 
 
 # Types for 'NodeNG.nodes_of_class()'
 _NodesT = TypeVar("_NodesT", bound="NodeNG")
 _NodesT2 = TypeVar("_NodesT2", bound="NodeNG")
@@ -76,15 +83,15 @@
     This is redefined in most concrete classes.
     """
     _other_fields: ClassVar[tuple[str, ...]] = ()
     """Node attributes that do not contain child nodes."""
     _other_other_fields: ClassVar[tuple[str, ...]] = ()
     """Attributes that contain AST-dependent fields."""
     # instance specific inference function infer(node, context)
-    _explicit_inference: InferFn | None = None
+    _explicit_inference: InferFn[Self] | None = None
 
     def __init__(
         self,
         lineno: int | None,
         col_offset: int | None,
         parent: NodeNG | None,
         *,
@@ -132,19 +139,28 @@
         :rtype: iterable
         """
         if context is not None:
             context = context.extra_context.get(self, context)
         if self._explicit_inference is not None:
             # explicit_inference is not bound, give it self explicitly
             try:
-                # pylint: disable=not-callable
-                results = list(self._explicit_inference(self, context, **kwargs))
-                if context is not None:
-                    context.nodes_inferred += len(results)
-                yield from results
+                if context is None:
+                    yield from self._explicit_inference(
+                        self,  # type: ignore[arg-type]
+                        context,
+                        **kwargs,
+                    )
+                    return
+                for result in self._explicit_inference(
+                    self,  # type: ignore[arg-type]
+                    context,
+                    **kwargs,
+                ):
+                    context.nodes_inferred += 1
+                    yield result
                 return
             except UseInferenceDefault:
                 pass
 
         if not context:
             # nodes_inferred?
             yield from self._infer(context=context, **kwargs)
@@ -170,28 +186,25 @@
             context.nodes_inferred += 1
 
         # Cache generated results for subsequent inferences of the
         # same node using the same context
         context.inferred[key] = tuple(results)
         return
 
-    def _repr_name(self) -> str:
+    def repr_name(self) -> str:
         """Get a name for nice representation.
 
         This is either :attr:`name`, :attr:`attrname`, or the empty string.
-
-        :returns: The nice name.
-        :rtype: str
         """
         if all(name not in self._astroid_fields for name in ("name", "attrname")):
             return getattr(self, "name", "") or getattr(self, "attrname", "")
         return ""
 
     def __str__(self) -> str:
-        rname = self._repr_name()
+        rname = self.repr_name()
         cname = type(self).__name__
         if rname:
             string = "%(cname)s.%(rname)s(%(fields)s)"
             alignment = len(cname) + len(rname) + 2
         else:
             string = "%(cname)s(%(fields)s)"
             alignment = len(cname) + 1
@@ -209,15 +222,15 @@
         return string % {
             "cname": cname,
             "rname": rname,
             "fields": (",\n" + " " * alignment).join(result),
         }
 
     def __repr__(self) -> str:
-        rname = self._repr_name()
+        rname = self.repr_name()
         if rname:
             string = "<%(cname)s.%(rname)s l.%(lineno)s at 0x%(id)x>"
         else:
             string = "<%(cname)s l.%(lineno)s at 0x%(id)x>"
         return string % {
             "cname": type(self).__name__,
             "rname": rname,
```

### Comparing `astroid-3.0.0a2/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.0.0a3/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/nodes/scoped_nodes/mixin.py` & `astroid-3.0.0a3/astroid/nodes/scoped_nodes/mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, TypeVar, overload
 
 from astroid.filter_statements import _filter_stmts
 from astroid.nodes import node_classes, scoped_nodes
 from astroid.nodes.scoped_nodes.utils import builtin_lookup
-from astroid.typing import SuccessfulInferenceResult
+from astroid.typing import InferenceResult, SuccessfulInferenceResult
 
 if TYPE_CHECKING:
     from astroid import nodes
 
 _T = TypeVar("_T")
 
 
@@ -23,15 +23,15 @@
     """this class provides locals handling common to Module, FunctionDef
     and ClassDef nodes, including a dict like interface for direct access
     to locals information
     """
 
     # attributes below are set by the builder module or by raw factories
 
-    locals: dict[str, list[SuccessfulInferenceResult]] = {}
+    locals: dict[str, list[InferenceResult]] = {}
     """A map of the name of a local variable to the node defining the local."""
 
     def qname(self) -> str:
         """Get the 'qualified' name of the node.
 
         For example: module.name, module.class.name ...
```

### Comparing `astroid-3.0.0a2/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.0.0a3/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1395,21 +1395,20 @@
         """
         # check we are defined in a ClassDef, because this is usually expected
         # (e.g. pylint...) when is_method() return True
         return self.type != "function" and isinstance(
             self.parent.frame(future=True), ClassDef
         )
 
-    def decoratornames(self, context: InferenceContext | None = None):
+    def decoratornames(self, context: InferenceContext | None = None) -> set[str]:
         """Get the qualified names of each of the decorators on this function.
 
         :param context:
             An inference context that can be passed to inference functions
         :returns: The names of the decorators.
-        :rtype: set(str)
         """
         result = set()
         decoratornodes = []
         if self.decorators is not None:
             decoratornodes += self.decorators.nodes
         decoratornodes += self.extra_decorators
         for decnode in decoratornodes:
@@ -1748,15 +1747,14 @@
         if klass.parent is None:
             klass = None
         else:
             klass = klass.parent.frame(future=True)
     return klass
 
 
-# pylint: disable=too-many-instance-attributes
 class ClassDef(
     _base_nodes.FilterStmtsBaseNode, LocalsDictNodeNG, _base_nodes.Statement
 ):
     """Class representing an :class:`ast.ClassDef` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
@@ -1817,15 +1815,15 @@
 
         self.keywords: list[node_classes.Keyword] = []
         """The keywords given to the class definition.
 
         This is usually for :pep:`3115` style metaclass declaration.
         """
 
-        self.bases: list[NodeNG] = []
+        self.bases: list[SuccessfulInferenceResult] = []
         """What the class inherits from."""
 
         self.body: list[NodeNG] = []
         """The contents of the class body."""
 
         self.name = name
         """The name of the class."""
@@ -1867,15 +1865,15 @@
         # __qualname__ is defined in PEP3155
         locals_ += (("__qualname__", self.special_attributes.attr___qualname__),)
         return locals_
 
     # pylint: disable=redefined-outer-name
     def postinit(
         self,
-        bases: list[NodeNG],
+        bases: list[SuccessfulInferenceResult],
         body: list[NodeNG],
         decorators: node_classes.Decorators | None,
         newstyle: bool | None = None,
         metaclass: NodeNG | None = None,
         keywords: list[node_classes.Keyword] | None = None,
         *,
         position: Position | None = None,
```

### Comparing `astroid-3.0.0a2/astroid/nodes/scoped_nodes/utils.py` & `astroid-3.0.0a3/astroid/nodes/scoped_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/objects.py` & `astroid-3.0.0a3/astroid/objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/protocols.py` & `astroid-3.0.0a3/astroid/protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/raw_building.py` & `astroid-3.0.0a3/astroid/raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/rebuilder.py` & `astroid-3.0.0a3/astroid/rebuilder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/scoped_nodes.py` & `astroid-3.0.0a3/astroid/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/test_utils.py` & `astroid-3.0.0a3/astroid/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid/transforms.py` & `astroid-3.0.0a3/astroid/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,22 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from collections.abc import Callable
 from typing import TYPE_CHECKING, List, Optional, Tuple, TypeVar, Union, cast, overload
 
 from astroid.context import _invalidate_cache
-from astroid.typing import SuccessfulInferenceResult
+from astroid.typing import SuccessfulInferenceResult, TransformFn
 
 if TYPE_CHECKING:
     from astroid import nodes
 
     _SuccessfulInferenceResultT = TypeVar(
         "_SuccessfulInferenceResultT", bound=SuccessfulInferenceResult
     )
-    _Transform = Callable[
-        [_SuccessfulInferenceResultT], Optional[SuccessfulInferenceResult]
-    ]
     _Predicate = Optional[Callable[[_SuccessfulInferenceResultT], bool]]
 
 _Vistables = Union[
     "nodes.NodeNG", List["nodes.NodeNG"], Tuple["nodes.NodeNG", ...], str, None
 ]
 _VisitReturns = Union[
     SuccessfulInferenceResult,
@@ -48,15 +45,15 @@
     def __init__(self) -> None:
         # The typing here is incorrect, but it's the best we can do
         # Refer to register_transform and unregister_transform for the correct types
         self.transforms: defaultdict[
             type[SuccessfulInferenceResult],
             list[
                 tuple[
-                    _Transform[SuccessfulInferenceResult],
+                    TransformFn[SuccessfulInferenceResult],
                     _Predicate[SuccessfulInferenceResult],
                 ]
             ],
         ] = defaultdict(list)
 
     def _transform(self, node: SuccessfulInferenceResult) -> SuccessfulInferenceResult:
         """Call matching transforms for the given node if any and return the
@@ -119,15 +116,15 @@
             return node
 
         return self._visit(node)
 
     def register_transform(
         self,
         node_class: type[_SuccessfulInferenceResultT],
-        transform: _Transform[_SuccessfulInferenceResultT],
+        transform: TransformFn[_SuccessfulInferenceResultT],
         predicate: _Predicate[_SuccessfulInferenceResultT] | None = None,
     ) -> None:
         """Register `transform(node)` function to be applied on the given node.
 
         The transform will only be applied if `predicate` is None or returns true
         when called with the node as argument.
 
@@ -135,20 +132,20 @@
         substitute the original node in the tree.
         """
         self.transforms[node_class].append((transform, predicate))  # type: ignore[index, arg-type]
 
     def unregister_transform(
         self,
         node_class: type[_SuccessfulInferenceResultT],
-        transform: _Transform[_SuccessfulInferenceResultT],
+        transform: TransformFn[_SuccessfulInferenceResultT],
         predicate: _Predicate[_SuccessfulInferenceResultT] | None = None,
     ) -> None:
         """Unregister the given transform."""
         self.transforms[node_class].remove((transform, predicate))  # type: ignore[index, arg-type]
 
-    def visit(self, module: nodes.Module) -> SuccessfulInferenceResult:
+    def visit(self, node: nodes.NodeNG) -> SuccessfulInferenceResult:
         """Walk the given astroid *tree* and transform each encountered node.
 
         Only the nodes which have transforms registered will actually
         be replaced or changed.
         """
-        return self._visit(module)
+        return self._visit(node)
```

### Comparing `astroid-3.0.0a2/astroid/typing.py` & `astroid-3.0.0a3/astroid/typing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Callable, Generator, TypedDict, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generator,
+    Generic,
+    Protocol,
+    TypedDict,
+    TypeVar,
+    Union,
+)
 
 if TYPE_CHECKING:
     from astroid import bases, exceptions, nodes, transforms, util
     from astroid.context import InferenceContext
     from astroid.interpreter._import import spec
 
 
-_NodesT = TypeVar("_NodesT", bound="nodes.NodeNG")
-
-
 class InferenceErrorInfo(TypedDict):
     """Store additional Inference error information
     raised with StopIteration exception.
     """
 
     node: nodes.NodeNG
     context: InferenceContext | None
 
 
-InferFn = Callable[..., Any]
-
-
 class AstroidManagerBrain(TypedDict):
     """Dictionary to store relevant information for a AstroidManager class."""
 
     astroid_cache: dict[str, nodes.Module]
     _mod_file_cache: dict[
         tuple[str, str | None], spec.ModuleSpec | exceptions.AstroidImportError
     ]
@@ -39,28 +43,55 @@
     optimize_ast: bool
     extension_package_whitelist: set[str]
     _transform: transforms.TransformVisitor
 
 
 InferenceResult = Union["nodes.NodeNG", "util.UninferableBase", "bases.Proxy"]
 SuccessfulInferenceResult = Union["nodes.NodeNG", "bases.Proxy"]
+_SuccessfulInferenceResultT = TypeVar(
+    "_SuccessfulInferenceResultT", bound=SuccessfulInferenceResult
+)
+_SuccessfulInferenceResultT_contra = TypeVar(
+    "_SuccessfulInferenceResultT_contra",
+    bound=SuccessfulInferenceResult,
+    contravariant=True,
+)
 
 ConstFactoryResult = Union[
     "nodes.List",
     "nodes.Set",
     "nodes.Tuple",
     "nodes.Dict",
     "nodes.Const",
     "nodes.EmptyNode",
 ]
 
 InferBinaryOp = Callable[
     [
-        Union[_NodesT, "bases.Instance"],
+        _SuccessfulInferenceResultT,
         Union["nodes.AugAssign", "nodes.BinOp"],
         str,
         InferenceResult,
         "InferenceContext",
         SuccessfulInferenceResult,
     ],
     Generator[InferenceResult, None, None],
 ]
+
+
+class InferFn(Protocol, Generic[_SuccessfulInferenceResultT_contra]):
+    def __call__(
+        self,
+        node: _SuccessfulInferenceResultT_contra,
+        context: InferenceContext | None = None,
+        **kwargs: Any,
+    ) -> Generator[InferenceResult, None, None]:
+        ...  # pragma: no cover
+
+
+class TransformFn(Protocol, Generic[_SuccessfulInferenceResultT]):
+    def __call__(
+        self,
+        node: _SuccessfulInferenceResultT,
+        infer_function: InferFn[_SuccessfulInferenceResultT] = ...,
+    ) -> _SuccessfulInferenceResultT | None:
+        ...  # pragma: no cover
```

### Comparing `astroid-3.0.0a2/astroid/util.py` & `astroid-3.0.0a3/astroid/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/astroid.egg-info/PKG-INFO` & `astroid-3.0.0a3/astroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a2/astroid.egg-info/SOURCES.txt` & `astroid-3.0.0a3/astroid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 astroid/typing.py
 astroid/util.py
 astroid.egg-info/PKG-INFO
 astroid.egg-info/SOURCES.txt
 astroid.egg-info/dependency_links.txt
 astroid.egg-info/requires.txt
 astroid.egg-info/top_level.txt
+astroid/../requirements_dev.txt
+astroid/../requirements_full.txt
+astroid/../requirements_minimal.txt
+astroid/../tox.ini
+astroid/../tests/__init__.py
+astroid/../tests/resources.py
 astroid/brain/__init__.py
 astroid/brain/brain_argparse.py
 astroid/brain/brain_attrs.py
 astroid/brain/brain_boto3.py
 astroid/brain/brain_builtin_inference.py
 astroid/brain/brain_collections.py
 astroid/brain/brain_crypt.py
```

### Comparing `astroid-3.0.0a2/pyproject.toml` & `astroid-3.0.0a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,22 @@
 
 [tool.setuptools]
 license-files = ["LICENSE", "CONTRIBUTORS.txt"]  # Keep in sync with setup.cfg
 
 [tool.setuptools.packages.find]
 include = ["astroid*"]
 
+[tool.setuptools.package-data]
+"*" = [
+    "../requirements*.txt",
+    "../tox.ini",
+    "../tests/__init__.py",
+    "../tests/resources.py",
+]
+
 [tool.setuptools.dynamic]
 version = {attr = "astroid.__pkginfo__.__version__"}
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
```

### Comparing `astroid-3.0.0a2/tests/test_builder.py` & `astroid-3.0.0a3/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_constraint.py` & `astroid-3.0.0a3/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_decorators.py` & `astroid-3.0.0a3/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_filter_statements.py` & `astroid-3.0.0a3/tests/test_filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_group_exceptions.py` & `astroid-3.0.0a3/tests/test_group_exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_helpers.py` & `astroid-3.0.0a3/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             ("1", self._extract("int")),
             ("[]", self._extract("list")),
             ("{1, 2, 3}", self._extract("set")),
             ("{1:2, 4:3}", self._extract("dict")),
             ("type", self._extract("type")),
             ("object", self._extract("type")),
             ("object()", self._extract("object")),
+            ("super()", self._extract("super")),
             ("lambda: None", self._build_custom_builtin("function")),
             ("len", self._build_custom_builtin("builtin_function_or_method")),
             ("None", self._build_custom_builtin("NoneType")),
             ("import sys\nsys#@", self._build_custom_builtin("module")),
         ]
         for code, expected in pairs:
             node = builder.extract_node(code)
@@ -254,7 +255,12 @@
         class A(type): #@
             pass
         """
         )
         builtin_type = self._extract("type")
         self.assertTrue(helpers.is_supertype(builtin_type, cls_a))
         self.assertTrue(helpers.is_subtype(cls_a, builtin_type))
+
+
+def test_uninferable_for_safe_infer() -> None:
+    uninfer = util.Uninferable
+    assert helpers.safe_infer(util.Uninferable) == uninfer
```

### Comparing `astroid-3.0.0a2/tests/test_inference.py` & `astroid-3.0.0a3/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_inference_calls.py` & `astroid-3.0.0a3/tests/test_inference_calls.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_lookup.py` & `astroid-3.0.0a3/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_manager.py` & `astroid-3.0.0a3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_modutils.py` & `astroid-3.0.0a3/tests/test_modutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 from astroid import modutils
 from astroid.const import PY310_PLUS
 from astroid.interpreter._import import spec
 
 from . import resources
 
 try:
-    import urllib3  # type: ignore[import]  # pylint: disable=unused-import
+    import urllib3  # type: ignore[import]
 
-    HAS_URLLIB3 = True
+    HAS_URLLIB3_V1 = urllib3.__version__.startswith("1")
 except ImportError:
-    HAS_URLLIB3 = False
+    HAS_URLLIB3_V1 = False
 
 
 def _get_file_from_object(obj) -> str:
     return modutils._path_from_filename(obj.__file__)
 
 
 class ModuleFileTest(unittest.TestCase):
@@ -543,16 +543,17 @@
         self.assertFalse(
             modutils.is_module_name_part_of_extension_package_whitelist(
                 "core.umath", {"numpy"}
             )
         )
 
 
-@pytest.mark.skipif(not HAS_URLLIB3, reason="This test requires urllib3.")
+@pytest.mark.skipif(not HAS_URLLIB3_V1, reason="This test requires urllib3 < 2.")
 def test_file_info_from_modpath__SixMetaPathImporter() -> None:
+    """Six is not backported anymore in urllib3 v2.0.0+"""
     assert modutils.file_info_from_modpath(["urllib3.packages.six.moves.http_client"])
 
 
 def test_find_setuptools_pep660_editable_install():
     """Find the spec for a package installed via setuptools PEP 660 import hooks."""
     # pylint: disable-next=import-outside-toplevel
     from tests.testdata.python3.data.import_setuptools_pep660.__editable___example_0_1_0_finder import (
```

### Comparing `astroid-3.0.0a2/tests/test_nodes.py` & `astroid-3.0.0a3/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_nodes_lineno.py` & `astroid-3.0.0a3/tests/test_nodes_lineno.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_nodes_position.py` & `astroid-3.0.0a3/tests/test_nodes_position.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_object_model.py` & `astroid-3.0.0a3/tests/test_object_model.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_objects.py` & `astroid-3.0.0a3/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_protocols.py` & `astroid-3.0.0a3/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_python3.py` & `astroid-3.0.0a3/tests/test_python3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_raw_building.py` & `astroid-3.0.0a3/tests/test_raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_regrtest.py` & `astroid-3.0.0a3/tests/test_regrtest.py`

 * *Files 6% similar despite different names*

```diff
@@ -332,14 +332,35 @@
                 pass
         """
         node = extract_node(code)
         inferred = next(node.infer())
         assert isinstance(inferred, Instance)
         assert inferred.qname() == ".A"
 
+    def test_inference_context_consideration(self) -> None:
+        """https://github.com/PyCQA/astroid/issues/1828"""
+        code = """
+        class Base:
+            def return_type(self):
+                return type(self)()
+        class A(Base):
+            def method(self):
+                return self.return_type()
+        class B(Base):
+            def method(self):
+                return self.return_type()
+        A().method() #@
+        B().method() #@
+        """
+        node1, node2 = extract_node(code)
+        inferred1 = next(node1.infer())
+        assert inferred1.qname() == ".A"
+        inferred2 = next(node2.infer())
+        assert inferred2.qname() == ".B"
+
 
 class Whatever:
     a = property(lambda x: x, lambda x: x)  # type: ignore[misc]
 
 
 def test_ancestor_looking_up_redefined_function() -> None:
     code = """
```

### Comparing `astroid-3.0.0a2/tests/test_scoped_nodes.py` & `astroid-3.0.0a3/tests/test_scoped_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1767,17 +1767,15 @@
         assert isinstance(cls, nodes.ClassDef)
         self.assertEqualMro(
             cls,
             [
                 "FinalClass",
                 "ClassB",
                 "MixinB",
-                # We don't recognize what 'cls' is at time of .format() call, only
-                # what it is at the end.
-                # "strMixin",
+                "strMixin",
                 "ClassA",
                 "MixinA",
                 "intMixin",
                 "Base",
                 "object",
             ],
         )
```

### Comparing `astroid-3.0.0a2/tests/test_stdlib.py` & `astroid-3.0.0a3/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_transforms.py` & `astroid-3.0.0a3/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a2/tests/test_utils.py` & `astroid-3.0.0a3/tests/test_utils.py`

 * *Files identical despite different names*

