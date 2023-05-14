# Comparing `tmp/flit_core-3.8.0.tar.gz` & `tmp/flit_core-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flit_core-3.8.0.tar", last modified: Sat Nov  5 13:07:59 2022, max compression
+gzip compressed data, was "flit_core-3.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flit_core-3.8.0.tar` & `flit_core-3.9.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0     1525 2022-11-05 12:52:43.629104 flit_core-3.8.0/LICENSE
--rw-r--r--   0        0        0     1742 2022-11-05 12:52:43.629104 flit_core-3.8.0/bootstrap_install.py
--rw-r--r--   0        0        0      421 2022-11-05 12:52:27.470017 flit_core-3.8.0/build_dists.py
--rw-r--r--   0        0        0      224 2022-11-05 13:06:27.382138 flit_core-3.8.0/flit_core/__init__.py
--rw-r--r--   0        0        0     3282 2021-11-14 14:34:30.346272 flit_core-3.8.0/flit_core/buildapi.py
--rw-r--r--   0        0        0    14520 2022-11-05 12:52:43.629104 flit_core-3.8.0/flit_core/common.py
--rw-r--r--   0        0        0    23247 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/config.py
--rw-r--r--   0        0        0     7045 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/sdist.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/__init__.py
--rw-r--r--   0        0        0      165 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/EG_README.rst
--rw-r--r--   0        0        0      221 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/bad-description-ext.toml
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/conflicting_modules/module1.py
--rw-r--r--   0        0        0      180 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/conflicting_modules/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/conflicting_modules/src/module1.py
--rw-r--r--   0        0        0      115 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/constructed_version/module1.py
--rw-r--r--   0        0        0      266 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/constructed_version/pyproject.toml
--rw-r--r--   0        0        0      305 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/extras-dev-conflict.toml
--rw-r--r--   0        0        0      361 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/extras.toml
--rw-r--r--   0        0        0      103 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/samples/imported_version/package1/__init__.py
--rw-r--r--   0        0        0       22 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/samples/imported_version/package1/_version.py
--rw-r--r--   0        0        0      220 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/samples/imported_version/pyproject.toml
--rw-r--r--   0        0        0      100 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/inclusion/LICENSES/README
--rw-r--r--   0        0        0        0 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/samples/inclusion/doc/subdir/subsubdir/test.md
--rw-r--r--   0        0        0       48 2021-11-14 14:34:30.347272 flit_core-3.8.0/flit_core/tests/samples/inclusion/doc/subdir/test.txt
--rw-r--r--   0        0        0       48 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/inclusion/doc/test.rst
--rw-r--r--   0        0        0       48 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/inclusion/doc/test.txt
--rw-r--r--   0        0        0       37 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/inclusion/module1.py
--rw-r--r--   0        0        0      239 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/samples/inclusion/pyproject.toml
--rw-r--r--   0        0        0       95 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/invalid_version1.py
--rw-r--r--   0        0        0      254 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/missing-description-file.toml
--rw-r--r--   0        0        0      299 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/misspelled-key.toml
--rw-r--r--   0        0        0      118 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/module1-pkg.ini
--rw-r--r--   0        0        0      288 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/module1-pkg.toml
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/module1.py
--rw-r--r--   0        0        0      187 2021-12-06 14:34:44.137786 flit_core-3.8.0/flit_core/tests/samples/module2.py
--rw-r--r--   0        0        0       80 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/moduleunimportable.py
--rw-r--r--   0        0        0      113 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/samples/moduleunimportabledouble.py
--rw-r--r--   0        0        0       29 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/my-description.rst
--rw-r--r--   0        0        0      303 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/no_docstring-pkg.toml
--rw-r--r--   0        0        0       20 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/no_docstring.py
--rw-r--r--   0        0        0        0 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/samples/normalization/my_python_module.py
--rw-r--r--   0        0        0      333 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/samples/normalization/pyproject.toml
--rw-r--r--   0        0        0      165 2021-11-18 22:10:43.577393 flit_core-3.8.0/flit_core/tests/samples/ns1-pkg/EG_README.rst
--rw-r--r--   0        0        0       76 2021-11-18 22:10:43.577393 flit_core-3.8.0/flit_core/tests/samples/ns1-pkg/ns1/pkg/__init__.py
--rw-r--r--   0        0        0      266 2021-11-18 22:10:43.577393 flit_core-3.8.0/flit_core/tests/samples/ns1-pkg/pyproject.toml
--rw-r--r--   0        0        0      311 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/package1.toml
--rw-r--r--   0        0        0       84 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/package1/__init__.py
--rw-r--r--   0        0        0       35 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/package1/data_dir/foo.sh
--rw-r--r--   0        0        0        6 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/package1/foo.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/package1/subpkg/__init__.py
--rw-r--r--   0        0        0       18 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/package1/subpkg/sp_data_dir/test.json
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/package1/subpkg2/__init__.py
--rw-r--r--   0        0        0       36 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/pep517/LICENSE
--rw-r--r--   0        0        0       37 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/pep517/README.rst
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.348272 flit_core-3.8.0/flit_core/tests/samples/pep517/module1.py
--rw-r--r--   0        0        0      380 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/pep517/pyproject.toml
--rw-r--r--   0        0        0       36 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/pep621/LICENSE
--rw-r--r--   0        0        0       37 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/pep621/README.rst
--rw-r--r--   0        0        0       42 2022-04-09 19:45:18.284031 flit_core-3.8.0/flit_core/tests/samples/pep621/module1a.py
--rw-r--r--   0        0        0      694 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/pep621/pyproject.toml
--rw-r--r--   0        0        0       37 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/pep621_nodynamic/README.rst
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/pep621_nodynamic/module1.py
--rw-r--r--   0        0        0      650 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/pep621_nodynamic/pyproject.toml
--rw-r--r--   0        0        0      311 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/requires-dev.toml
--rw-r--r--   0        0        0      252 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/requires-envmark.toml
--rw-r--r--   0        0        0      299 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/requires-extra-envmark.toml
--rw-r--r--   0        0        0      239 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/samples/requires-requests.toml
--rw-r--r--   0        0        0       36 2022-11-05 12:52:27.545017 flit_core-3.8.0/flit_core/tests/samples/with_data_dir/LICENSE
--rw-r--r--   0        0        0       37 2022-11-05 12:52:27.545017 flit_core-3.8.0/flit_core/tests/samples/with_data_dir/README.rst
--rw-r--r--   0        0        0       18 2022-11-05 12:52:27.545017 flit_core-3.8.0/flit_core/tests/samples/with_data_dir/data/share/man/man1/foo.1
--rw-r--r--   0        0        0       42 2022-11-05 12:52:27.545017 flit_core-3.8.0/flit_core/tests/samples/with_data_dir/module1.py
--rw-r--r--   0        0        0      452 2022-11-05 12:52:27.545017 flit_core-3.8.0/flit_core/tests/samples/with_data_dir/pyproject.toml
--rw-r--r--   0        0        0     1552 2022-11-05 12:52:27.470017 flit_core-3.8.0/flit_core/tests/test_build_thyself.py
--rw-r--r--   0        0        0     3934 2021-11-14 14:34:30.349272 flit_core-3.8.0/flit_core/tests/test_buildapi.py
--rw-r--r--   0        0        0     5951 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/test_common.py
--rw-r--r--   0        0        0     7316 2022-11-05 12:52:43.630104 flit_core-3.8.0/flit_core/tests/test_config.py
--rw-r--r--   0        0        0     1941 2022-11-05 12:52:43.631104 flit_core-3.8.0/flit_core/tests/test_sdist.py
--rw-r--r--   0        0        0     1170 2021-11-14 14:34:30.350272 flit_core-3.8.0/flit_core/tests/test_versionno.py
--rw-r--r--   0        0        0     1716 2022-11-05 12:52:43.631104 flit_core-3.8.0/flit_core/tests/test_wheel.py
--rw-r--r--   0        0        0      791 2022-11-05 12:52:27.463017 flit_core-3.8.0/flit_core/vendor/README
--rw-r--r--   0        0        0        0 2022-11-05 12:52:27.447017 flit_core-3.8.0/flit_core/vendor/__init__.py
--rw-r--r--   0        0        0     1072 2022-11-05 12:52:27.452017 flit_core-3.8.0/flit_core/vendor/tomli-1.2.3.dist-info/LICENSE
--rw-r--r--   0        0        0     9089 2022-11-05 12:52:27.452017 flit_core-3.8.0/flit_core/vendor/tomli-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      294 2022-11-05 12:52:27.452017 flit_core-3.8.0/flit_core/vendor/tomli/__init__.py
--rw-r--r--   0        0        0    21649 2022-11-05 12:52:27.452017 flit_core-3.8.0/flit_core/vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2813 2022-11-05 12:52:27.452017 flit_core-3.8.0/flit_core/vendor/tomli/_re.py
--rw-r--r--   0        0        0      126 2022-11-05 12:52:27.452017 flit_core-3.8.0/flit_core/vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2022-11-05 12:52:27.452017 flit_core-3.8.0/flit_core/vendor/tomli/py.typed
--rw-r--r--   0        0        0     4781 2021-11-14 14:34:30.350272 flit_core-3.8.0/flit_core/versionno.py
--rw-r--r--   0        0        0     9269 2022-11-05 12:52:43.631104 flit_core-3.8.0/flit_core/wheel.py
--rw-r--r--   0        0        0      651 2022-11-05 12:52:43.631104 flit_core-3.8.0/pyproject.toml
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 flit_core-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1525 2023-05-14 14:43:38.926691 flit_core-3.9.0/LICENSE
+-rw-r--r--   0        0        0      333 2023-05-14 14:43:38.926691 flit_core-3.9.0/README.rst
+-rw-r--r--   0        0        0     1742 2023-05-14 14:43:38.926691 flit_core-3.9.0/bootstrap_install.py
+-rw-r--r--   0        0        0      421 2023-05-14 14:43:38.926691 flit_core-3.9.0/build_dists.py
+-rw-r--r--   0        0        0      224 2023-05-14 14:47:29.185487 flit_core-3.9.0/flit_core/__init__.py
+-rw-r--r--   0        0        0     3282 2021-11-14 14:34:30.346272 flit_core-3.9.0/flit_core/buildapi.py
+-rw-r--r--   0        0        0    15145 2023-05-14 14:43:38.927691 flit_core-3.9.0/flit_core/common.py
+-rw-r--r--   0        0        0    23247 2023-05-14 14:43:38.927691 flit_core-3.9.0/flit_core/config.py
+-rw-r--r--   0        0        0     7237 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/sdist.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/__init__.py
+-rw-r--r--   0        0        0      165 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/EG_README.rst
+-rw-r--r--   0        0        0      221 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/bad-description-ext.toml
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/conflicting_modules/module1.py
+-rw-r--r--   0        0        0      180 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/conflicting_modules/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/conflicting_modules/src/module1.py
+-rw-r--r--   0        0        0      115 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/constructed_version/module1.py
+-rw-r--r--   0        0        0      266 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/constructed_version/pyproject.toml
+-rw-r--r--   0        0        0      305 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/extras-dev-conflict.toml
+-rw-r--r--   0        0        0      361 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/extras.toml
+-rw-r--r--   0        0        0      138 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/tests/samples/imported_version/package1/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/tests/samples/imported_version/package1/_version.py
+-rw-r--r--   0        0        0      220 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/tests/samples/imported_version/pyproject.toml
+-rw-r--r--   0        0        0      100 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/inclusion/LICENSES/README
+-rw-r--r--   0        0        0        0 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/tests/samples/inclusion/doc/subdir/subsubdir/test.md
+-rw-r--r--   0        0        0       48 2021-11-14 14:34:30.347272 flit_core-3.9.0/flit_core/tests/samples/inclusion/doc/subdir/test.txt
+-rw-r--r--   0        0        0       48 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/inclusion/doc/test.rst
+-rw-r--r--   0        0        0       48 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/inclusion/doc/test.txt
+-rw-r--r--   0        0        0       37 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/inclusion/module1.py
+-rw-r--r--   0        0        0      239 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/tests/samples/inclusion/pyproject.toml
+-rw-r--r--   0        0        0       95 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/invalid_version1.py
+-rw-r--r--   0        0        0      254 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/missing-description-file.toml
+-rw-r--r--   0        0        0      299 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/misspelled-key.toml
+-rw-r--r--   0        0        0      118 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/module1-pkg.ini
+-rw-r--r--   0        0        0      288 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/module1-pkg.toml
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/module1.py
+-rw-r--r--   0        0        0      187 2021-12-06 14:34:44.137786 flit_core-3.9.0/flit_core/tests/samples/module2.py
+-rw-r--r--   0        0        0       80 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/moduleunimportable.py
+-rw-r--r--   0        0        0      113 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/tests/samples/moduleunimportabledouble.py
+-rw-r--r--   0        0        0       29 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/my-description.rst
+-rw-r--r--   0        0        0      303 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/no_docstring-pkg.toml
+-rw-r--r--   0        0        0       20 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/no_docstring.py
+-rw-r--r--   0        0        0        0 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/tests/samples/normalization/my_python_module.py
+-rw-r--r--   0        0        0      334 2023-05-14 14:43:38.928691 flit_core-3.9.0/flit_core/tests/samples/normalization/pyproject.toml
+-rw-r--r--   0        0        0      165 2021-11-18 22:10:43.577393 flit_core-3.9.0/flit_core/tests/samples/ns1-pkg/EG_README.rst
+-rw-r--r--   0        0        0       76 2021-11-18 22:10:43.577393 flit_core-3.9.0/flit_core/tests/samples/ns1-pkg/ns1/pkg/__init__.py
+-rw-r--r--   0        0        0      266 2021-11-18 22:10:43.577393 flit_core-3.9.0/flit_core/tests/samples/ns1-pkg/pyproject.toml
+-rw-r--r--   0        0        0      311 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/package1.toml
+-rw-r--r--   0        0        0       84 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/package1/__init__.py
+-rw-r--r--   0        0        0       35 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/package1/data_dir/foo.sh
+-rw-r--r--   0        0        0        6 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/package1/foo.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/package1/subpkg/__init__.py
+-rw-r--r--   0        0        0       18 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/package1/subpkg/sp_data_dir/test.json
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/package1/subpkg2/__init__.py
+-rw-r--r--   0        0        0       36 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/pep517/LICENSE
+-rw-r--r--   0        0        0       37 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/pep517/README.rst
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.348272 flit_core-3.9.0/flit_core/tests/samples/pep517/module1.py
+-rw-r--r--   0        0        0      380 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/pep517/pyproject.toml
+-rw-r--r--   0        0        0       36 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/pep621/LICENSE
+-rw-r--r--   0        0        0       37 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/pep621/README.rst
+-rw-r--r--   0        0        0       42 2022-04-09 19:45:18.284031 flit_core-3.9.0/flit_core/tests/samples/pep621/module1a.py
+-rw-r--r--   0        0        0      694 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/pep621/pyproject.toml
+-rw-r--r--   0        0        0       37 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/pep621_nodynamic/README.rst
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/pep621_nodynamic/module1.py
+-rw-r--r--   0        0        0      650 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/pep621_nodynamic/pyproject.toml
+-rw-r--r--   0        0        0      311 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/requires-dev.toml
+-rw-r--r--   0        0        0      252 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/requires-envmark.toml
+-rw-r--r--   0        0        0      299 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/requires-extra-envmark.toml
+-rw-r--r--   0        0        0      239 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/samples/requires-requests.toml
+-rw-r--r--   0        0        0       36 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/samples/with_data_dir/LICENSE
+-rw-r--r--   0        0        0       37 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/samples/with_data_dir/README.rst
+-rw-r--r--   0        0        0       18 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/samples/with_data_dir/data/share/man/man1/foo.1
+-rw-r--r--   0        0        0       42 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/samples/with_data_dir/module1.py
+-rw-r--r--   0        0        0      452 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/samples/with_data_dir/pyproject.toml
+-rw-r--r--   0        0        0     1552 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/test_build_thyself.py
+-rw-r--r--   0        0        0     3934 2021-11-14 14:34:30.349272 flit_core-3.9.0/flit_core/tests/test_buildapi.py
+-rw-r--r--   0        0        0     5951 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/test_common.py
+-rw-r--r--   0        0        0     7316 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/test_config.py
+-rw-r--r--   0        0        0     2202 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/test_sdist.py
+-rw-r--r--   0        0        0     1170 2021-11-14 14:34:30.350272 flit_core-3.9.0/flit_core/tests/test_versionno.py
+-rw-r--r--   0        0        0     1716 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/tests/test_wheel.py
+-rw-r--r--   0        0        0      791 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/vendor/README
+-rw-r--r--   0        0        0        0 2023-05-14 14:43:38.929691 flit_core-3.9.0/flit_core/vendor/__init__.py
+-rw-r--r--   0        0        0     1072 2023-05-14 14:43:38.930691 flit_core-3.9.0/flit_core/vendor/tomli-1.2.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     9089 2023-05-14 14:43:38.930691 flit_core-3.9.0/flit_core/vendor/tomli-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      294 2023-05-14 14:43:38.930691 flit_core-3.9.0/flit_core/vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    21649 2023-05-14 14:43:38.930691 flit_core-3.9.0/flit_core/vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2813 2023-05-14 14:43:38.930691 flit_core-3.9.0/flit_core/vendor/tomli/_re.py
+-rw-r--r--   0        0        0      126 2023-05-14 14:43:38.930691 flit_core-3.9.0/flit_core/vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2023-05-14 14:43:38.930691 flit_core-3.9.0/flit_core/vendor/tomli/py.typed
+-rw-r--r--   0        0        0     4781 2021-11-14 14:34:30.350272 flit_core-3.9.0/flit_core/versionno.py
+-rw-r--r--   0        0        0     9306 2023-05-14 14:43:38.930691 flit_core-3.9.0/flit_core/wheel.py
+-rw-r--r--   0        0        0      712 2023-05-14 14:43:38.931691 flit_core-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 flit_core-3.9.0/PKG-INFO
```

### Comparing `flit_core-3.8.0/LICENSE` & `flit_core-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/bootstrap_install.py` & `flit_core-3.9.0/bootstrap_install.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/buildapi.py` & `flit_core-3.9.0/flit_core/buildapi.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/common.py` & `flit_core-3.9.0/flit_core/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,29 @@
     @property
     def file(self):
         if self.is_package:
             return self.path / '__init__.py'
         else:
             return self.path
 
+    @property
+    def version_files(self):
+        """Files which will be parsed to find a version number
+
+        Files later in this list take precedence over earlier ones.
+        """
+        if self.is_package:
+            paths = [self.path / '__init__.py']
+            for filename in ('version.py', '_version.py', '__version__.py'):
+                if (self.path / filename).is_file():
+                    paths.insert(0, self.path / filename)
+            return paths
+        else:
+            return [self.path]
+
     def iter_files(self):
         """Iterate over the files contained in this module.
 
         Yields absolute paths - caller may want to make them relative.
         Excludes any __pycache__ and *.pyc files.
         """
         def _include(path):
@@ -123,34 +138,34 @@
         logging.root.handlers = logging_handlers
 
 def get_docstring_and_version_via_ast(target):
     """
     Return a tuple like (docstring, version) for the given module,
     extracted by parsing its AST.
     """
-    # read as bytes to enable custom encodings
-    with target.file.open('rb') as f:
-        node = ast.parse(f.read())
-    for child in node.body:
-        # Only use the version from the given module if it's a simple
-        # string assignment to __version__
-        is_version_str = (
-                isinstance(child, ast.Assign)
-                and any(
-                    isinstance(target, ast.Name)
-                    and target.id == "__version__"
-                    for target in child.targets
-                )
-                and isinstance(child.value, ast.Str)
-        )
-        if is_version_str:
-            version = child.value.s
-            break
-    else:
-        version = None
+    version = None
+    for target_path in target.version_files:
+        # read as bytes to enable custom encodings
+        with target_path.open('rb') as f:
+            node = ast.parse(f.read())
+        for child in node.body:
+            # Only use the version from the given module if it's a simple
+            # string assignment to __version__
+            is_version_str = (
+                    isinstance(child, ast.Assign)
+                    and any(
+                        isinstance(target, ast.Name)
+                        and target.id == "__version__"
+                        for target in child.targets
+                    )
+                    and isinstance(child.value, ast.Str)
+            )
+            if is_version_str:
+                version = child.value.s
+                break
     return ast.get_docstring(node), version
 
 
 # To ensure we're actually loading the specified file, give it a unique name to
 # avoid any cached import. In normal use we'll only load one module per process,
 # so it should only matter for the tests, but we'll do it anyway.
 _import_i = 0
```

### Comparing `flit_core-3.8.0/flit_core/config.py` & `flit_core-3.9.0/flit_core/config.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/sdist.py` & `flit_core-3.9.0/flit_core/sdist.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,24 +153,25 @@
 
     def add_setup_py(self, files_to_add, target_tarfile):
         """No-op here; overridden in flit to generate setup.py"""
         pass
 
     @property
     def dir_name(self):
-        return '{}-{}'.format(self.metadata.name, self.metadata.version)
+        return common.normalize_dist_name(self.metadata.name, self.metadata.version)
 
     def build(self, target_dir, gen_setup_py=True):
         os.makedirs(str(target_dir), exist_ok=True)
-        target = target_dir / '{}-{}.tar.gz'.format(
-                self.metadata.name, self.metadata.version
-        )
+        target = target_dir / '{}.tar.gz'.format(self.dir_name)
         source_date_epoch = os.environ.get('SOURCE_DATE_EPOCH', '')
         mtime = int(source_date_epoch) if source_date_epoch else None
-        gz = GzipFile(str(target), mode='wb', mtime=mtime)
+        # For the gzip timestamp, default to 2016-1-1 00:00 (UTC)
+        # This makes the sdist reproducible even without SOURCE_DATE_EPOCH,
+        # if the source file mtimes don't change, i.e. from the same checkout.
+        gz = GzipFile(str(target), mode='wb', mtime=(mtime or 1451606400))
         tf = tarfile.TarFile(str(target), mode='w', fileobj=gz,
                              format=tarfile.PAX_FORMAT)
 
         try:
             files_to_add = self.apply_includes_excludes(self.select_files())
 
             for relpath in files_to_add:
```

### Comparing `flit_core-3.8.0/flit_core/tests/samples/pep621/pyproject.toml` & `flit_core-3.9.0/flit_core/tests/samples/pep621/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/tests/samples/pep621_nodynamic/pyproject.toml` & `flit_core-3.9.0/flit_core/tests/samples/pep621_nodynamic/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/tests/test_build_thyself.py` & `flit_core-3.9.0/flit_core/tests/test_build_thyself.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/tests/test_buildapi.py` & `flit_core-3.9.0/flit_core/tests/test_buildapi.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/tests/test_common.py` & `flit_core-3.9.0/flit_core/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/tests/test_config.py` & `flit_core-3.9.0/flit_core/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/tests/test_sdist.py` & `flit_core-3.9.0/flit_core/tests/test_sdist.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,7 +55,16 @@
 def test_data_dir():
     builder = sdist.SdistBuilder.from_ini_path(
         samples_dir / 'with_data_dir' / 'pyproject.toml'
     )
     files = builder.apply_includes_excludes(builder.select_files())
 
     assert osp.join('data', 'share', 'man', 'man1', 'foo.1') in files
+
+
+def test_pep625(tmp_path):
+    builder = sdist.SdistBuilder.from_ini_path(
+        samples_dir / 'normalization' / 'pyproject.toml'
+    )
+    path = builder.build(tmp_path)
+    assert path == tmp_path / 'my_python_module-0.0.1.tar.gz'
+    assert_isfile(path)
```

### Comparing `flit_core-3.8.0/flit_core/tests/test_versionno.py` & `flit_core-3.9.0/flit_core/tests/test_versionno.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/tests/test_wheel.py` & `flit_core-3.9.0/flit_core/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/vendor/README` & `flit_core-3.9.0/flit_core/vendor/README`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/vendor/tomli-1.2.3.dist-info/LICENSE` & `flit_core-3.9.0/flit_core/vendor/tomli-1.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/vendor/tomli-1.2.3.dist-info/METADATA` & `flit_core-3.9.0/flit_core/vendor/tomli-1.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/vendor/tomli/_parser.py` & `flit_core-3.9.0/flit_core/vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/vendor/tomli/_re.py` & `flit_core-3.9.0/flit_core/vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/versionno.py` & `flit_core-3.9.0/flit_core/versionno.py`

 * *Files identical despite different names*

### Comparing `flit_core-3.8.0/flit_core/wheel.py` & `flit_core-3.9.0/flit_core/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     f.write(wheel_file_template)
     if supports_py2:
         f.write(u"Tag: py2-none-any\n")
     f.write(u"Tag: py3-none-any\n")
 
 
 def _set_zinfo_mode(zinfo, mode):
-    # Set the bits for the mode and bit 0xFFFF for “regular file”
+    # Set the bits for the mode
     zinfo.external_attr = mode << 16
 
 
 def zip_timestamp_from_env() -> Optional[tuple]:
     """Prepare a timestamp from $SOURCE_DATE_EPOCH, if set"""
     try:
         # If SOURCE_DATE_EPOCH is set (e.g. by Debian), it's used for
@@ -143,15 +143,16 @@
 
         log.debug("Writing data to %s in zip file", rel_path)
         # The default is a fixed timestamp rather than the current time, so
         # that building a wheel twice on the same computer can automatically
         # give you the exact same result.
         date_time = self.source_time_stamp or (2016, 1, 1, 0, 0, 0)
         zi = zipfile.ZipInfo(rel_path, date_time)
-        _set_zinfo_mode(zi, mode)
+        # Also sets bit 0x8000 for "regular file" (S_IFREG)
+        _set_zinfo_mode(zi, mode | stat.S_IFREG)
         b = sio.getvalue().encode('utf-8')
         hashsum = hashlib.sha256(b)
         hash_digest = urlsafe_b64encode(hashsum.digest()).decode('ascii').rstrip('=')
         self.wheel_zip.writestr(zi, b, compress_type=zipfile.ZIP_DEFLATED)
         self.records.append((rel_path, hash_digest, len(b)))
 
     def copy_module(self):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flit_core-3.8.0/pyproject.toml` & `flit_core-3.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 name="flit_core"
 authors=[
     {name = "Thomas Kluyver & contributors", email = "thomas@kluyver.me.uk"},
 ]
 description = "Distribution-building parts of Flit. See flit package for more information"
 dependencies = []
 requires-python = '>=3.6'
+readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = ["version"]
 
 [project.urls]
+Documentation = "https://flit.pypa.io"
 Source = "https://github.com/pypa/flit"
 
 [tool.flit.sdist]
 include = ["bootstrap_install.py", "build_dists.py"]
```

