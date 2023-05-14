# Comparing `tmp/astroid-3.0.0a1.tar.gz` & `tmp/astroid-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-3.0.0a1.tar", last modified: Tue Apr 25 12:17:50 2023, max compression
+gzip compressed data, was "astroid-3.0.0a2.tar", last modified: Tue Apr 25 17:57:05 2023, max compression
```

## Comparing `astroid-3.0.0a1.tar` & `astroid-3.0.0a2.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.646873 astroid-3.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-25 12:17:30.000000 astroid-3.0.0a1/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-25 12:17:30.000000 astroid-3.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 12:17:30.000000 astroid-3.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 12:17:50.646873 astroid-3.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-25 12:17:30.000000 astroid-3.0.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.622873 astroid-3.0.0a1/astroid/
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/_backport_stdlib_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26368 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.634873 astroid-3.0.0a1/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    34564 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23321 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    45131 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.634873 astroid-3.0.0a1/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.638873 astroid-3.0.0a1/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    33517 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23500 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.638873 astroid-3.0.0a1/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (123)   136648 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.638873 astroid-3.0.0a1/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/scoped_nodes/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)   103259 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/scoped_nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-25 12:17:30.000000 astroid-3.0.0a1/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.626873 astroid-3.0.0a1/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 12:17:50.000000 astroid-3.0.0a1/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-25 12:17:30.000000 astroid-3.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 12:17:50.646873 astroid-3.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:17:50.646873 astroid-3.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_group_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)   221738 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_inference_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21514 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    63153 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_nodes_lineno.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_nodes_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_python3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_regrtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    96027 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-25 12:17:30.000000 astroid-3.0.0a1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.480415 astroid-3.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-25 17:56:48.000000 astroid-3.0.0a2/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-25 17:56:48.000000 astroid-3.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 17:56:48.000000 astroid-3.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 17:57:05.480415 astroid-3.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-25 17:56:48.000000 astroid-3.0.0a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.464414 astroid-3.0.0a2/astroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26368 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.472415 astroid-3.0.0a2/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34564 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23321 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45131 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.472415 astroid-3.0.0a2/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.472415 astroid-3.0.0a2/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33517 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23500 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.476415 astroid-3.0.0a2/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134011 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.476415 astroid-3.0.0a2/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100986 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-25 17:56:48.000000 astroid-3.0.0a2/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.464414 astroid-3.0.0a2/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 17:57:05.000000 astroid-3.0.0a2/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-25 17:56:48.000000 astroid-3.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 17:57:05.480415 astroid-3.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:57:05.480415 astroid-3.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   221608 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21514 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61209 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92916 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-25 17:56:48.000000 astroid-3.0.0a2/tests/test_utils.py
```

### Comparing `astroid-3.0.0a1/CONTRIBUTORS.txt` & `astroid-3.0.0a2/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/LICENSE` & `astroid-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/PKG-INFO` & `astroid-3.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a1/README.rst` & `astroid-3.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/__init__.py` & `astroid-3.0.0a2/astroid/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 # isort: off
 # It's impossible to import from astroid.nodes with a wildcard, because
 # there is a cyclic import that prevent creating an __all__ in astroid/nodes
 # and we need astroid/scoped_nodes and astroid/node_classes to work. So
 # importing with a wildcard would clash with astroid/nodes/scoped_nodes
 # and astroid/nodes/node_classes.
-from astroid.nodes import (  # pylint: disable=redefined-builtin (Ellipsis)
+from astroid.nodes import (
     CONST_CLS,
     AnnAssign,
     Arguments,
     Assert,
     Assign,
     AssignAttr,
     AssignName,
@@ -113,30 +113,27 @@
     Decorators,
     DelAttr,
     Delete,
     DelName,
     Dict,
     DictComp,
     DictUnpack,
-    Ellipsis,
     EmptyNode,
     EvaluatedObject,
     ExceptHandler,
     Expr,
-    ExtSlice,
     For,
     FormattedValue,
     FunctionDef,
     GeneratorExp,
     Global,
     If,
     IfExp,
     Import,
     ImportFrom,
-    Index,
     JoinedStr,
     Keyword,
     Lambda,
     List,
     ListComp,
     Match,
     MatchAs,
```

### Comparing `astroid-3.0.0a1/astroid/_ast.py` & `astroid-3.0.0a2/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/_backport_stdlib_names.py` & `astroid-3.0.0a2/astroid/_backport_stdlib_names.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/arguments.py` & `astroid-3.0.0a2/astroid/arguments.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/astroid_manager.py` & `astroid-3.0.0a2/astroid/astroid_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/bases.py` & `astroid-3.0.0a2/astroid/bases.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_argparse.py` & `astroid-3.0.0a2/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_attrs.py` & `astroid-3.0.0a2/astroid/brain/brain_attrs.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_boto3.py` & `astroid-3.0.0a2/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_builtin_inference.py` & `astroid-3.0.0a2/astroid/brain/brain_builtin_inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_collections.py` & `astroid-3.0.0a2/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_crypt.py` & `astroid-3.0.0a2/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_ctypes.py` & `astroid-3.0.0a2/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_curses.py` & `astroid-3.0.0a2/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_dataclasses.py` & `astroid-3.0.0a2/astroid/brain/brain_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_dateutil.py` & `astroid-3.0.0a2/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_fstrings.py` & `astroid-3.0.0a2/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_functools.py` & `astroid-3.0.0a2/astroid/brain/brain_functools.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_gi.py` & `astroid-3.0.0a2/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_hashlib.py` & `astroid-3.0.0a2/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_http.py` & `astroid-3.0.0a2/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_hypothesis.py` & `astroid-3.0.0a2/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_io.py` & `astroid-3.0.0a2/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_mechanize.py` & `astroid-3.0.0a2/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_multiprocessing.py` & `astroid-3.0.0a2/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.0.0a2/astroid/brain/brain_namedtuple_enum.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_nose.py` & `astroid-3.0.0a2/astroid/brain/brain_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_core_einsumfunc.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_ma.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_numpy_utils.py` & `astroid-3.0.0a2/astroid/brain/brain_numpy_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_pathlib.py` & `astroid-3.0.0a2/astroid/brain/brain_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_pkg_resources.py` & `astroid-3.0.0a2/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_pytest.py` & `astroid-3.0.0a2/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_qt.py` & `astroid-3.0.0a2/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_random.py` & `astroid-3.0.0a2/astroid/brain/brain_random.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_re.py` & `astroid-3.0.0a2/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_regex.py` & `astroid-3.0.0a2/astroid/brain/brain_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_responses.py` & `astroid-3.0.0a2/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_scipy_signal.py` & `astroid-3.0.0a2/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_signal.py` & `astroid-3.0.0a2/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_six.py` & `astroid-3.0.0a2/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_sqlalchemy.py` & `astroid-3.0.0a2/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_ssl.py` & `astroid-3.0.0a2/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_subprocess.py` & `astroid-3.0.0a2/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_threading.py` & `astroid-3.0.0a2/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_type.py` & `astroid-3.0.0a2/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_typing.py` & `astroid-3.0.0a2/astroid/brain/brain_typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_unittest.py` & `astroid-3.0.0a2/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/brain_uuid.py` & `astroid-3.0.0a2/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/brain/helpers.py` & `astroid-3.0.0a2/astroid/brain/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/builder.py` & `astroid-3.0.0a2/astroid/builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/const.py` & `astroid-3.0.0a2/astroid/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/constraint.py` & `astroid-3.0.0a2/astroid/constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/context.py` & `astroid-3.0.0a2/astroid/context.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/decorators.py` & `astroid-3.0.0a2/astroid/decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/exceptions.py` & `astroid-3.0.0a2/astroid/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/filter_statements.py` & `astroid-3.0.0a2/astroid/filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/helpers.py` & `astroid-3.0.0a2/astroid/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/inference.py` & `astroid-3.0.0a2/astroid/inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/inference_tip.py` & `astroid-3.0.0a2/astroid/inference_tip.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/interpreter/_import/spec.py` & `astroid-3.0.0a2/astroid/interpreter/_import/spec.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/interpreter/_import/util.py` & `astroid-3.0.0a2/astroid/interpreter/_import/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/interpreter/dunder_lookup.py` & `astroid-3.0.0a2/astroid/interpreter/dunder_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/interpreter/objectmodel.py` & `astroid-3.0.0a2/astroid/interpreter/objectmodel.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/manager.py` & `astroid-3.0.0a2/astroid/manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/mixins.py` & `astroid-3.0.0a2/astroid/mixins.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/modutils.py` & `astroid-3.0.0a2/astroid/modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/node_classes.py` & `astroid-3.0.0a2/astroid/node_classes.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # For details: https://github.com/pylint-dev/astroid/blob/main/LICENSE
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 # pylint: disable=unused-import
 
 import warnings
 
-from astroid.nodes.node_classes import (  # pylint: disable=redefined-builtin (Ellipsis)
+from astroid.nodes.node_classes import (
     CONST_CLS,
     AnnAssign,
     Arguments,
     Assert,
     Assign,
     AssignAttr,
     AssignName,
@@ -30,28 +30,25 @@
     Continue,
     Decorators,
     DelAttr,
     Delete,
     DelName,
     Dict,
     DictUnpack,
-    Ellipsis,
     EmptyNode,
     EvaluatedObject,
     ExceptHandler,
     Expr,
-    ExtSlice,
     For,
     FormattedValue,
     Global,
     If,
     IfExp,
     Import,
     ImportFrom,
-    Index,
     JoinedStr,
     Keyword,
     List,
     LookupMixIn,
     Match,
     MatchAs,
     MatchCase,
```

### Comparing `astroid-3.0.0a1/astroid/nodes/__init__.py` & `astroid-3.0.0a2/astroid/nodes/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 # Nodes not present in the builtin ast module:  DictUnpack, Unknown, and EvaluatedObject.
 
 # This is the only node we re-export from the private _base_nodes module. This
 # is because it was originally part of the public API and hasn't been deprecated.
 from astroid.nodes._base_nodes import Statement
-from astroid.nodes.node_classes import (  # pylint: disable=redefined-builtin (Ellipsis)
+from astroid.nodes.node_classes import (
     CONST_CLS,
     AnnAssign,
     Arguments,
     Assert,
     Assign,
     AssignAttr,
     AssignName,
@@ -39,28 +39,25 @@
     Continue,
     Decorators,
     DelAttr,
     Delete,
     DelName,
     Dict,
     DictUnpack,
-    Ellipsis,
     EmptyNode,
     EvaluatedObject,
     ExceptHandler,
     Expr,
-    ExtSlice,
     For,
     FormattedValue,
     Global,
     If,
     IfExp,
     Import,
     ImportFrom,
-    Index,
     JoinedStr,
     Keyword,
     List,
     Match,
     MatchAs,
     MatchCase,
     MatchClass,
@@ -145,30 +142,27 @@
     Decorators,
     DelAttr,
     Delete,
     DelName,
     Dict,
     DictComp,
     DictUnpack,
-    Ellipsis,
     EmptyNode,
     EvaluatedObject,
     ExceptHandler,
     Expr,
-    ExtSlice,
     For,
     FormattedValue,
     FunctionDef,
     GeneratorExp,
     Global,
     If,
     IfExp,
     Import,
     ImportFrom,
-    Index,
     JoinedStr,
     Keyword,
     Lambda,
     List,
     ListComp,
     LocalsDictNodeNG,
     Match,
@@ -237,32 +231,29 @@
     "Decorators",
     "DelAttr",
     "Delete",
     "DelName",
     "Dict",
     "DictComp",
     "DictUnpack",
-    "Ellipsis",
     "EmptyNode",
     "EvaluatedObject",
     "ExceptHandler",
     "Expr",
-    "ExtSlice",
     "For",
     "FormattedValue",
     "FunctionDef",
     "function_to_method",
     "GeneratorExp",
     "get_wrapping_class",
     "Global",
     "If",
     "IfExp",
     "Import",
     "ImportFrom",
-    "Index",
     "JoinedStr",
     "Keyword",
     "Lambda",
     "List",
     "ListComp",
     "LocalsDictNodeNG",
     "Match",
```

### Comparing `astroid-3.0.0a1/astroid/nodes/_base_nodes.py` & `astroid-3.0.0a2/astroid/nodes/_base_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/nodes/as_string.py` & `astroid-3.0.0a2/astroid/nodes/as_string.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/nodes/const.py` & `astroid-3.0.0a2/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/nodes/node_classes.py` & `astroid-3.0.0a2/astroid/nodes/node_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """Module for some node classes. More nodes in scoped_nodes.py"""
 
 from __future__ import annotations
 
 import abc
 import itertools
 import typing
-import warnings
 from collections.abc import Generator, Iterable, Iterator, Mapping
 from functools import cached_property, lru_cache
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
@@ -2031,24 +2030,14 @@
         yield self.value
 
     def _get_yield_nodes_skip_lambdas(self):
         if not self.value.is_lambda:
             yield from self.value._get_yield_nodes_skip_lambdas()
 
 
-class Ellipsis(_base_nodes.NoChildrenNode):  # pylint: disable=redefined-builtin
-    """Class representing an :class:`ast.Ellipsis` node.
-
-    An :class:`Ellipsis` is the ``...`` syntax.
-
-    Deprecated since v2.6.0 - Use :class:`Const` instead.
-    Will be removed with the release v2.7.0
-    """
-
-
 class EmptyNode(_base_nodes.NoChildrenNode):
     """Holds an arbitrary object in the :attr:`LocalsDictNodeNG.locals`."""
 
     object = None
 
     def __init__(
         self,
@@ -2145,24 +2134,14 @@
         :param exceptions: The names of the exceptions to check for.
         """
         if self.type is None or exceptions is None:
             return True
         return any(node.name in exceptions for node in self.type._get_name_nodes())
 
 
-class ExtSlice(NodeNG):
-    """Class representing an :class:`ast.ExtSlice` node.
-
-    An :class:`ExtSlice` is a complex slice expression.
-
-    Deprecated since v2.6.0 - Now part of the :class:`Subscript` node.
-    Will be removed with the release of v2.7.0
-    """
-
-
 class For(
     _base_nodes.MultiLineWithElseBlockNode,
     _base_nodes.AssignTypeNode,
     _base_nodes.Statement,
 ):
     """Class representing an :class:`ast.For` node.
 
@@ -2499,67 +2478,14 @@
         return len(self.orelse) == 1 and isinstance(self.orelse[0], If)
 
     def _get_yield_nodes_skip_lambdas(self):
         """An If node can contain a Yield node in the test"""
         yield from self.test._get_yield_nodes_skip_lambdas()
         yield from super()._get_yield_nodes_skip_lambdas()
 
-    def is_sys_guard(self) -> bool:
-        """Return True if IF stmt is a sys.version_info guard.
-
-        >>> import astroid
-        >>> node = astroid.extract_node('''
-        import sys
-        if sys.version_info > (3, 8):
-            from typing import Literal
-        else:
-            from typing_extensions import Literal
-        ''')
-        >>> node.is_sys_guard()
-        True
-        """
-        warnings.warn(
-            "The 'is_sys_guard' function is deprecated and will be removed in astroid 3.0.0 "
-            "It has been moved to pylint and can be imported from 'pylint.checkers.utils' "
-            "starting with pylint 2.12",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        if isinstance(self.test, Compare):
-            value = self.test.left
-            if isinstance(value, Subscript):
-                value = value.value
-            if isinstance(value, Attribute) and value.as_string() == "sys.version_info":
-                return True
-
-        return False
-
-    def is_typing_guard(self) -> bool:
-        """Return True if IF stmt is a typing guard.
-
-        >>> import astroid
-        >>> node = astroid.extract_node('''
-        from typing import TYPE_CHECKING
-        if TYPE_CHECKING:
-            from xyz import a
-        ''')
-        >>> node.is_typing_guard()
-        True
-        """
-        warnings.warn(
-            "The 'is_typing_guard' function is deprecated and will be removed in astroid 3.0.0 "
-            "It has been moved to pylint and can be imported from 'pylint.checkers.utils' "
-            "starting with pylint 2.12",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return isinstance(
-            self.test, (Name, Attribute)
-        ) and self.test.as_string().endswith("TYPE_CHECKING")
-
 
 class IfExp(NodeNG):
     """Class representing an :class:`ast.IfExp` node.
     >>> import astroid
     >>> node = astroid.extract_node('value if condition else other')
     >>> node
     <IfExp l.1 at 0x7f23b2e9dbe0>
@@ -2640,24 +2566,14 @@
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
 
-class Index(NodeNG):
-    """Class representing an :class:`ast.Index` node.
-
-    An :class:`Index` is a simple subscript.
-
-    Deprecated since v2.6.0 - Now part of the :class:`Subscript` node.
-    Will be removed with the release of v2.7.0
-    """
-
-
 class Keyword(NodeNG):
     """Class representing an :class:`ast.keyword` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('function(a_kwarg=True)')
     >>> node
     <Call l.1 at 0x7f23b2e9e320>
```

### Comparing `astroid-3.0.0a1/astroid/nodes/node_ng.py` & `astroid-3.0.0a2/astroid/nodes/node_ng.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.0.0a2/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/nodes/scoped_nodes/mixin.py` & `astroid-3.0.0a2/astroid/nodes/scoped_nodes/mixin.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.0.0a2/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,14 @@
 
     # names of module attributes available through the global scope
     scope_attrs = {"__name__", "__doc__", "__file__", "__path__", "__package__"}
     """The names of module attributes available through the global scope."""
 
     _other_fields = (
         "name",
-        "doc",
         "file",
         "path",
         "package",
         "pure_python",
         "future_imports",
     )
     _other_other_fields = ("locals", "globals")
@@ -217,17 +216,14 @@
         path: Sequence[str] | None = None,
         package: bool = False,
         pure_python: bool = True,
     ) -> None:
         self.name = name
         """The name of the module."""
 
-        self._doc: str | None = None
-        """The module docstring."""
-
         self.file = file
         """The path to the file that this ast has been extracted from.
 
         This will be ``None`` when the representation has been built from a
         built-in module.
         """
 
@@ -258,37 +254,14 @@
     # pylint: enable=redefined-builtin
 
     def postinit(
         self, body: list[node_classes.NodeNG], *, doc_node: Const | None = None
     ):
         self.body = body
         self.doc_node = doc_node
-        if doc_node:
-            self._doc = doc_node.value
-
-    @property
-    def doc(self) -> str | None:
-        """The module docstring."""
-        warnings.warn(
-            "The 'Module.doc' attribute is deprecated, "
-            "use 'Module.doc_node' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self._doc
-
-    @doc.setter
-    def doc(self, value: str | None) -> None:
-        warnings.warn(
-            "Setting the 'Module.doc' attribute is deprecated, "
-            "use 'Module.doc_node' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self._doc = value
 
     def _get_stream(self):
         if self.file_bytes is not None:
             return io.BytesIO(self.file_bytes)
         if self.file is not None:
             # pylint: disable=consider-using-with
             stream = open(self.file, "rb")
@@ -1111,15 +1084,15 @@
     """
     If present, this will contain the type annotation for arguments
     passed by a type comment
     """
     type_comment_returns = None
     """If present, this will contain the return type annotation, passed by a type comment"""
     # attributes below are set by the builder module or by raw factories
-    _other_fields = ("name", "doc", "position")
+    _other_fields = ("name", "position")
     _other_other_fields = (
         "locals",
         "_type",
         "type_comment_returns",
         "type_comment_args",
     )
     _type = None
@@ -1140,17 +1113,14 @@
         *,
         end_lineno: int | None,
         end_col_offset: int | None,
     ) -> None:
         self.name = name
         """The name of the function."""
 
-        self._doc: str | None = None
-        """DEPRECATED: The function docstring."""
-
         self.locals = {}
         """A map of the name of a local variable to the node defining it."""
 
         self.body: list[NodeNG] = []
         """The contents of the function body."""
 
         self.instance_attrs: dict[str, list[NodeNG]] = {}
@@ -1199,37 +1169,14 @@
         self.body = body
         self.decorators = decorators
         self.returns = returns
         self.type_comment_returns = type_comment_returns
         self.type_comment_args = type_comment_args
         self.position = position
         self.doc_node = doc_node
-        if doc_node:
-            self._doc = doc_node.value
-
-    @property
-    def doc(self) -> str | None:
-        """The function docstring."""
-        warnings.warn(
-            "The 'FunctionDef.doc' attribute is deprecated, "
-            "use 'FunctionDef.doc_node' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self._doc
-
-    @doc.setter
-    def doc(self, value: str | None) -> None:
-        warnings.warn(
-            "Setting the 'FunctionDef.doc' attribute is deprecated, "
-            "use 'FunctionDef.doc_node' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self._doc = value
 
     @cached_property
     def extra_decorators(self) -> list[node_classes.Call]:
         """The extra decorators that this function can have.
 
         Additional decorators are considered when they are used as
         assignments, as in ``method = staticmethod(method)``.
@@ -1846,15 +1793,15 @@
         _class_type,
         doc=(
             "The class type for this node.\n\n"
             "Possible values are: class, metaclass, exception.\n\n"
             ":type: str"
         ),
     )
-    _other_fields = ("name", "doc", "is_dataclass", "position")
+    _other_fields = ("name", "is_dataclass", "position")
     _other_other_fields = ("locals", "_newstyle")
     _newstyle: bool | None = None
 
     def __init__(
         self,
         name: str,
         lineno: int,
@@ -1882,17 +1829,14 @@
 
         self.name = name
         """The name of the class."""
 
         self.decorators = None
         """The decorators that are applied to this class."""
 
-        self._doc: str | None = None
-        """DEPRECATED: The class docstring."""
-
         self.doc_node: Const | None = None
         """The doc node associated with this node."""
 
         self.is_dataclass: bool = False
         """Whether this class is a dataclass."""
 
         super().__init__(
@@ -1906,35 +1850,14 @@
             parent.frame(future=True).set_local(name, self)
 
         for local_name, node in self.implicit_locals():
             self.add_local_node(node, local_name)
 
     infer_binary_op: ClassVar[InferBinaryOp[ClassDef]]
 
-    @property
-    def doc(self) -> str | None:
-        """The class docstring."""
-        warnings.warn(
-            "The 'ClassDef.doc' attribute is deprecated, "
-            "use 'ClassDef.doc_node' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self._doc
-
-    @doc.setter
-    def doc(self, value: str | None) -> None:
-        warnings.warn(
-            "Setting the 'ClassDef.doc' attribute is deprecated, "
-            "use 'ClassDef.doc_node.value' instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self._doc = value
-
     def implicit_parameters(self) -> Literal[1]:
         return 1
 
     def implicit_locals(self):
         """Get implicitly defined class definition locals.
 
         :returns: the the name and Const pair for each local
@@ -1963,16 +1886,14 @@
         self.bases = bases
         self.body = body
         self.decorators = decorators
         self._newstyle = newstyle
         self._metaclass = metaclass
         self.position = position
         self.doc_node = doc_node
-        if doc_node:
-            self._doc = doc_node.value
 
     def _newstyle_impl(self, context: InferenceContext | None = None):
         if context is None:
             context = InferenceContext()
         if self._newstyle is not None:
             return self._newstyle
         for base in self.ancestors(recurs=False, context=context):
```

### Comparing `astroid-3.0.0a1/astroid/nodes/scoped_nodes/utils.py` & `astroid-3.0.0a2/astroid/nodes/scoped_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/objects.py` & `astroid-3.0.0a2/astroid/objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/protocols.py` & `astroid-3.0.0a2/astroid/protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/raw_building.py` & `astroid-3.0.0a2/astroid/raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/rebuilder.py` & `astroid-3.0.0a2/astroid/rebuilder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/scoped_nodes.py` & `astroid-3.0.0a2/astroid/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/test_utils.py` & `astroid-3.0.0a2/astroid/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/transforms.py` & `astroid-3.0.0a2/astroid/transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/typing.py` & `astroid-3.0.0a2/astroid/typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid/util.py` & `astroid-3.0.0a2/astroid/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/astroid.egg-info/PKG-INFO` & `astroid-3.0.0a2/astroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a1/astroid.egg-info/SOURCES.txt` & `astroid-3.0.0a2/astroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/pyproject.toml` & `astroid-3.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_builder.py` & `astroid-3.0.0a2/tests/test_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,17 +747,14 @@
     def setUp(self) -> None:
         self.module = resources.build_file("data/module.py", "data.module")
 
     def test_module_base_props(self) -> None:
         """Test base properties and method of an astroid module."""
         module = self.module
         self.assertEqual(module.name, "data.module")
-        with pytest.warns(DeprecationWarning) as records:
-            self.assertEqual(module.doc, "test module for astroid\n")
-            assert len(records) == 1
         assert isinstance(module.doc_node, nodes.Const)
         self.assertEqual(module.doc_node.value, "test module for astroid\n")
         self.assertEqual(module.fromlineno, 0)
         self.assertIsNone(module.parent)
         self.assertEqual(module.frame(), module)
         self.assertEqual(module.frame(future=True), module)
         self.assertEqual(module.root(), module)
@@ -793,17 +790,14 @@
         self.assertEqual(keys, sorted(should))
 
     def test_function_base_props(self) -> None:
         """Test base properties and method of an astroid function."""
         module = self.module
         function = module["global_access"]
         self.assertEqual(function.name, "global_access")
-        with pytest.warns(DeprecationWarning) as records:
-            self.assertEqual(function.doc, "function test")
-            assert len(records)
         assert isinstance(function.doc_node, nodes.Const)
         self.assertEqual(function.doc_node.value, "function test")
         self.assertEqual(function.fromlineno, 11)
         self.assertTrue(function.parent)
         self.assertEqual(function.frame(), function)
         self.assertEqual(function.parent.frame(), module)
         self.assertEqual(function.frame(future=True), function)
@@ -820,17 +814,14 @@
         self.assertEqual(keys, ["i", "key", "local", "val"])
 
     def test_class_base_props(self) -> None:
         """Test base properties and method of an astroid class."""
         module = self.module
         klass = module["YO"]
         self.assertEqual(klass.name, "YO")
-        with pytest.warns(DeprecationWarning) as records:
-            self.assertEqual(klass.doc, "hehe\n    haha")
-            assert len(records) == 1
         assert isinstance(klass.doc_node, nodes.Const)
         self.assertEqual(klass.doc_node.value, "hehe\n    haha")
         self.assertEqual(klass.fromlineno, 25)
         self.assertTrue(klass.parent)
         self.assertEqual(klass.frame(), klass)
         self.assertEqual(klass.parent.frame(), module)
         self.assertEqual(klass.frame(future=True), klass)
@@ -878,17 +869,14 @@
     def test_method_base_props(self) -> None:
         """Test base properties and method of an astroid method."""
         klass2 = self.module["YOUPI"]
         # "normal" method
         method = klass2["method"]
         self.assertEqual(method.name, "method")
         self.assertEqual([n.name for n in method.args.args], ["self"])
-        with pytest.warns(DeprecationWarning) as records:
-            self.assertEqual(method.doc, "method\n        test")
-            assert len(records) == 1
         assert isinstance(method.doc_node, nodes.Const)
         self.assertEqual(method.doc_node.value, "method\n        test")
         self.assertEqual(method.fromlineno, 48)
         self.assertEqual(method.type, "method")
         # class method
         method = klass2["class_method"]
         self.assertEqual([n.name for n in method.args.args], ["cls"])
```

### Comparing `astroid-3.0.0a1/tests/test_constraint.py` & `astroid-3.0.0a2/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_decorators.py` & `astroid-3.0.0a2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_filter_statements.py` & `astroid-3.0.0a2/tests/test_filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_group_exceptions.py` & `astroid-3.0.0a2/tests/test_group_exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_helpers.py` & `astroid-3.0.0a2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_inference.py` & `astroid-3.0.0a2/tests/test_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -6436,17 +6436,14 @@
     A.test #@
     """
     node = extract_node(code)
     inferred = next(node.infer())
     assert isinstance(inferred, objects.Property)
     assert isinstance(inferred.doc_node, nodes.Const)
     assert inferred.doc_node.value == "Docstring"
-    with pytest.warns(DeprecationWarning) as records:
-        assert inferred.doc == "Docstring"
-        assert len(records) == 1
 
 
 def test_recursion_error_inferring_builtin_containers() -> None:
     node = extract_node(
         """
     class Foo:
         a = "foo"
```

### Comparing `astroid-3.0.0a1/tests/test_inference_calls.py` & `astroid-3.0.0a2/tests/test_inference_calls.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_lookup.py` & `astroid-3.0.0a2/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_manager.py` & `astroid-3.0.0a2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_modutils.py` & `astroid-3.0.0a2/tests/test_modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_nodes.py` & `astroid-3.0.0a2/tests/test_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,74 +334,14 @@
         self.assertEqual(self.astroid.block_range(1), (0, 22))
         self.assertEqual(self.astroid.block_range(10), (0, 22))  # XXX (10, 22) ?
         self.assertEqual(self.astroid.body[1].block_range(5), (5, 6))
         self.assertEqual(self.astroid.body[1].block_range(6), (6, 6))
         self.assertEqual(self.astroid.body[1].orelse[0].block_range(7), (7, 8))
         self.assertEqual(self.astroid.body[1].orelse[0].block_range(8), (8, 8))
 
-    @staticmethod
-    @pytest.mark.filterwarnings("ignore:.*is_sys_guard:DeprecationWarning")
-    def test_if_sys_guard() -> None:
-        code = builder.extract_node(
-            """
-        import sys
-        if sys.version_info > (3, 8):  #@
-            pass
-
-        if sys.version_info[:2] > (3, 8):  #@
-            pass
-
-        if sys.some_other_function > (3, 8):  #@
-            pass
-        """
-        )
-        assert isinstance(code, list) and len(code) == 3
-
-        assert isinstance(code[0], nodes.If)
-        assert code[0].is_sys_guard() is True
-        assert isinstance(code[1], nodes.If)
-        assert code[1].is_sys_guard() is True
-
-        assert isinstance(code[2], nodes.If)
-        assert code[2].is_sys_guard() is False
-
-    @staticmethod
-    @pytest.mark.filterwarnings("ignore:.*is_typing_guard:DeprecationWarning")
-    def test_if_typing_guard() -> None:
-        code = builder.extract_node(
-            """
-        import typing
-        import typing as t
-        from typing import TYPE_CHECKING
-
-        if typing.TYPE_CHECKING:  #@
-            pass
-
-        if t.TYPE_CHECKING:  #@
-            pass
-
-        if TYPE_CHECKING:  #@
-            pass
-
-        if typing.SOME_OTHER_CONST:  #@
-            pass
-        """
-        )
-        assert isinstance(code, list) and len(code) == 4
-
-        assert isinstance(code[0], nodes.If)
-        assert code[0].is_typing_guard() is True
-        assert isinstance(code[1], nodes.If)
-        assert code[1].is_typing_guard() is True
-        assert isinstance(code[2], nodes.If)
-        assert code[2].is_typing_guard() is True
-
-        assert isinstance(code[3], nodes.If)
-        assert code[3].is_typing_guard() is False
-
 
 class TryExceptNodeTest(_NodeTest):
     CODE = """
         try:
             print ('pouet')
         except IOError:
             pass
@@ -1591,17 +1531,14 @@
         """\
     def func():
         "Docstring"
         return 1
     """
     )
     node: nodes.FunctionDef = astroid.extract_node(code)  # type: ignore[assignment]
-    with pytest.warns(DeprecationWarning) as records:
-        assert node.doc == "Docstring"
-        assert len(records) == 1
     assert isinstance(node.doc_node, nodes.Const)
     assert node.doc_node.value == "Docstring"
     assert node.doc_node.lineno == 2
     assert node.doc_node.col_offset == 4
     assert node.doc_node.end_lineno == 2
     assert node.doc_node.end_col_offset == 15
 
@@ -1609,17 +1546,14 @@
         """\
     def func():
         ...
         return 1
     """
     )
     node = astroid.extract_node(code)
-    with pytest.warns(DeprecationWarning) as records:
-        assert node.doc is None
-        assert len(records) == 1
     assert node.doc_node is None
 
 
 @test_utils.require_version(minver="3.8")
 def test_parse_fstring_debug_mode() -> None:
     node = astroid.extract_node('f"{3=}"')
     assert isinstance(node, nodes.JoinedStr)
```

### Comparing `astroid-3.0.0a1/tests/test_nodes_lineno.py` & `astroid-3.0.0a2/tests/test_nodes_lineno.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_nodes_position.py` & `astroid-3.0.0a2/tests/test_nodes_position.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_object_model.py` & `astroid-3.0.0a2/tests/test_object_model.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_objects.py` & `astroid-3.0.0a2/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_protocols.py` & `astroid-3.0.0a2/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_python3.py` & `astroid-3.0.0a2/tests/test_python3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_raw_building.py` & `astroid-3.0.0a2/tests/test_raw_building.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,25 +46,19 @@
         self.assertEqual(node.pure_python, False)
         self.assertEqual(node.package, False)
         self.assertEqual(node.parent, None)
 
     def test_build_class(self) -> None:
         node = build_class("MyClass")
         self.assertEqual(node.name, "MyClass")
-        with pytest.warns(DeprecationWarning) as records:
-            self.assertEqual(node.doc, None)
-            assert len(records) == 1
         self.assertEqual(node.doc_node, None)
 
     def test_build_function(self) -> None:
         node = build_function("MyFunction")
         self.assertEqual(node.name, "MyFunction")
-        with pytest.warns(DeprecationWarning) as records:
-            self.assertEqual(node.doc, None)
-            assert len(records) == 1
         self.assertEqual(node.doc_node, None)
 
     def test_build_function_args(self) -> None:
         args = ["myArgs1", "myArgs2"]
         node = build_function("MyFunction", args)
         self.assertEqual("myArgs1", node.args.args[0].name)
         self.assertEqual("myArgs2", node.args.args[1].name)
```

### Comparing `astroid-3.0.0a1/tests/test_regrtest.py` & `astroid-3.0.0a2/tests/test_regrtest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_scoped_nodes.py` & `astroid-3.0.0a2/tests/test_scoped_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from __future__ import annotations
 
 import datetime
 import os
 import sys
 import textwrap
 import unittest
-import warnings
 from functools import partial
 from typing import Any
 
 import pytest
 
 from astroid import (
     MANAGER,
@@ -987,17 +986,14 @@
             self.assertRaises(AttributeInferenceError, cls.getattr, "__mro__")
         for cls in (nodes.List._proxied, nodes.Const(1)._proxied):
             self.assertEqual(len(cls.getattr("__bases__")), 1)
             self.assertEqual(len(cls.getattr("__name__")), 1)
             self.assertEqual(
                 len(cls.getattr("__doc__")), 1, (cls, cls.getattr("__doc__"))
             )
-            with pytest.warns(DeprecationWarning) as records:
-                self.assertEqual(cls.getattr("__doc__")[0].value, cls.doc)
-                assert len(records) == 1
             self.assertEqual(cls.getattr("__doc__")[0].value, cls.doc_node.value)
             self.assertEqual(len(cls.getattr("__module__")), 4)
             self.assertEqual(len(cls.getattr("__dict__")), 1)
             self.assertEqual(len(cls.getattr("__mro__")), 1)
 
     def test__mro__attribute(self) -> None:
         node = builder.extract_node(
@@ -2845,96 +2841,7 @@
         """
         )
         assert module.body[0].frame() == module
         assert module.body[0].frame(future=True) == module
 
         assert module.body[1].value.locals["x"][0].frame() == module
         assert module.body[1].value.locals["x"][0].frame(future=True) == module
-
-
-def test_deprecation_of_doc_attribute() -> None:
-    code = textwrap.dedent(
-        """\
-    def func():
-        "Docstring"
-        return 1
-    """
-    )
-    node: nodes.FunctionDef = extract_node(code)  # type: ignore[assignment]
-    with pytest.warns(DeprecationWarning) as records:
-        assert node.doc == "Docstring"
-        assert len(records) == 1
-    with pytest.warns(DeprecationWarning) as records:
-        node.doc = None
-        assert len(records) == 1
-
-    code = textwrap.dedent(
-        """\
-    class MyClass():
-        '''Docstring'''
-    """
-    )
-    node: nodes.ClassDef = extract_node(code)  # type: ignore[assignment]
-    with pytest.warns(DeprecationWarning) as records:
-        assert node.doc == "Docstring"
-        assert len(records) == 1
-    with pytest.warns(DeprecationWarning) as records:
-        node.doc = None
-        assert len(records) == 1
-
-    code = textwrap.dedent(
-        """\
-    '''Docstring'''
-    """
-    )
-    node = parse(code)
-    with pytest.warns(DeprecationWarning) as records:
-        assert node.doc == "Docstring"
-        assert len(records) == 1
-    with pytest.warns(DeprecationWarning) as records:
-        node.doc = None
-        assert len(records) == 1
-
-    # If 'doc' isn't passed to Module, ClassDef, FunctionDef,
-    # no DeprecationWarning should be raised
-    doc_node = nodes.Const("Docstring")
-    with warnings.catch_warnings():
-        # Modify warnings filter to raise error for DeprecationWarning
-        warnings.simplefilter("error", DeprecationWarning)
-        node_module = nodes.Module(name="MyModule")
-        node_module.postinit(body=[], doc_node=doc_node)
-        assert node_module.doc_node == doc_node
-        node_class = nodes.ClassDef(
-            name="MyClass",
-            lineno=0,
-            col_offset=0,
-            end_lineno=0,
-            end_col_offset=0,
-            parent=nodes.Unknown(),
-        )
-        node_class.postinit(bases=[], body=[], decorators=[], doc_node=doc_node)
-        assert node_class.doc_node == doc_node
-        node_func = nodes.FunctionDef(
-            name="MyFunction",
-            lineno=0,
-            col_offset=0,
-            parent=node_module,
-            end_lineno=0,
-            end_col_offset=0,
-        )
-        node_func.postinit(
-            args=nodes.Arguments(parent=node_func, vararg=None, kwarg=None),
-            body=[],
-            doc_node=doc_node,
-        )
-        assert node_func.doc_node == doc_node
-
-    # Test 'doc' attribute if only 'doc_node' is passed
-    with pytest.warns(DeprecationWarning) as records:
-        assert node_module.doc == "Docstring"
-        assert len(records) == 1
-    with pytest.warns(DeprecationWarning) as records:
-        assert node_class.doc == "Docstring"
-        assert len(records) == 1
-    with pytest.warns(DeprecationWarning) as records:
-        assert node_func.doc == "Docstring"
-        assert len(records) == 1
```

### Comparing `astroid-3.0.0a1/tests/test_stdlib.py` & `astroid-3.0.0a2/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_transforms.py` & `astroid-3.0.0a2/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a1/tests/test_utils.py` & `astroid-3.0.0a2/tests/test_utils.py`

 * *Files identical despite different names*

