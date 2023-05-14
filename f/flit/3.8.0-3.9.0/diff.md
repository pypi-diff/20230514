# Comparing `tmp/flit-3.8.0.tar.gz` & `tmp/flit-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flit-3.8.0.tar", last modified: Sat Nov  5 13:08:51 2022, max compression
+gzip compressed data, was "flit-3.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flit-3.8.0.tar` & `flit-3.9.0.tar`

### file list

```diff
@@ -1,243 +1,244 @@
--rw-r--r--   0        0        0      295 2022-11-05 13:06:27.383138 flit-3.8.0/.bumpversion.cfg
--rw-r--r--   0        0        0       48 2022-11-05 12:52:27.480017 flit-3.8.0/.coveragerc
--rw-r--r--   0        0        0      117 2022-11-05 12:52:43.628104 flit-3.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0      890 2022-11-05 12:52:43.628104 flit-3.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      207 2021-11-18 22:10:43.574393 flit-3.8.0/.gitignore
--rw-r--r--   0        0        0     1525 2021-05-09 15:40:19.101348 flit-3.8.0/LICENSE
--rw-r--r--   0        0        0     2565 2022-11-05 12:27:30.176410 flit-3.8.0/README.rst
--rw-r--r--   0        0        0     1044 2022-11-05 12:52:27.470017 flit-3.8.0/bootstrap_dev.py
--rw-r--r--   0        0        0       13 2021-05-09 15:40:19.102348 flit-3.8.0/codecov.yml
--rw-r--r--   0        0        0     6754 2021-05-09 15:40:19.102348 flit-3.8.0/doc/Makefile
--rw-r--r--   0        0        0     8893 2021-05-09 15:40:19.102348 flit-3.8.0/doc/_static/flit_logo_nobg.svg
--rw-r--r--   0        0        0     5890 2021-05-09 15:40:19.102348 flit-3.8.0/doc/_static/flit_logo_nobg_cropped.png
--rw-r--r--   0        0        0     9141 2021-05-09 15:40:19.102348 flit-3.8.0/doc/_static/flit_logo_nobg_cropped.svg
--rw-r--r--   0        0        0     1735 2022-11-05 12:52:43.628104 flit-3.8.0/doc/bootstrap.rst
--rw-r--r--   0        0        0     7890 2022-11-05 13:06:10.847054 flit-3.8.0/doc/cmdline.rst
--rw-r--r--   0        0        0     8306 2022-11-05 13:06:27.383138 flit-3.8.0/doc/conf.py
--rw-r--r--   0        0        0      585 2022-11-05 12:52:43.628104 flit-3.8.0/doc/development.rst
--rw-r--r--   0        0        0     3422 2021-12-06 14:34:44.136786 flit-3.8.0/doc/flit_ini.rst
--rw-r--r--   0        0        0    20948 2022-11-05 13:06:10.847054 flit-3.8.0/doc/history.rst
--rw-r--r--   0        0        0      451 2021-11-14 14:34:30.343272 flit-3.8.0/doc/index.rst
--rw-r--r--   0        0        0     6697 2021-05-09 15:40:19.103348 flit-3.8.0/doc/make.bat
--rw-r--r--   0        0        0    15961 2022-11-05 13:06:10.848055 flit-3.8.0/doc/pyproject_toml.rst
--rw-r--r--   0        0        0     2829 2021-11-14 14:34:30.343272 flit-3.8.0/doc/rationale.rst
--rw-r--r--   0        0        0     1396 2021-05-09 15:40:19.103348 flit-3.8.0/doc/reproducible.rst
--rw-r--r--   0        0        0       70 2021-11-14 14:34:30.344272 flit-3.8.0/doc/requirements.txt
--rw-r--r--   0        0        0     2853 2021-11-14 14:34:30.344272 flit-3.8.0/doc/upload.rst
--rw-r--r--   0        0        0     8509 2022-11-05 13:06:27.381138 flit-3.8.0/flit/__init__.py
--rw-r--r--   0        0        0       68 2021-05-09 15:40:19.103348 flit-3.8.0/flit/__main__.py
--rw-r--r--   0        0        0      898 2021-05-09 15:40:19.103348 flit-3.8.0/flit/_get_dirs.py
--rw-r--r--   0        0        0     2120 2021-11-14 14:34:30.344272 flit-3.8.0/flit/build.py
--rw-r--r--   0        0        0       33 2021-11-14 14:34:30.344272 flit-3.8.0/flit/buildapi.py
--rw-r--r--   0        0        0      592 2021-11-14 14:34:30.344272 flit-3.8.0/flit/config.py
--rw-r--r--   0        0        0     9093 2021-11-14 14:34:30.344272 flit-3.8.0/flit/init.py
--rw-r--r--   0        0        0    16799 2022-11-05 12:52:27.539017 flit-3.8.0/flit/install.py
--rw-r--r--   0        0        0     9161 2021-05-09 15:40:19.104348 flit-3.8.0/flit/license_templates/apache
--rw-r--r--   0        0        0    32422 2021-05-09 15:40:19.104348 flit-3.8.0/flit/license_templates/gpl3
--rw-r--r--   0        0        0     1077 2021-05-09 15:40:19.104348 flit-3.8.0/flit/license_templates/mit
--rw-r--r--   0        0        0     4048 2021-05-09 15:40:19.104348 flit-3.8.0/flit/log.py
--rw-r--r--   0        0        0      468 2021-05-09 15:40:19.104348 flit-3.8.0/flit/logo.py
--rw-r--r--   0        0        0     8047 2021-11-18 22:10:43.575393 flit-3.8.0/flit/sdist.py
--rw-r--r--   0        0        0     2297 2021-11-14 14:34:30.345272 flit-3.8.0/flit/tomlify.py
--rw-r--r--   0        0        0     9296 2022-11-05 12:52:43.629104 flit-3.8.0/flit/upload.py
--rw-r--r--   0        0        0    10032 2021-11-14 14:34:30.345272 flit-3.8.0/flit/validate.py
--rw-r--r--   0        0        0      314 2021-11-14 14:34:30.346272 flit-3.8.0/flit/vcs/__init__.py
--rw-r--r--   0        0        0      574 2021-11-14 14:34:30.346272 flit-3.8.0/flit/vcs/git.py
--rw-r--r--   0        0        0     1258 2022-11-05 12:52:43.629104 flit-3.8.0/flit/vcs/hg.py
--rw-r--r--   0        0        0        0 2021-05-09 15:40:19.104348 flit-3.8.0/flit/vendorized/__init__.py
--rw-r--r--   0        0        0        0 2021-05-09 15:40:19.105348 flit-3.8.0/flit/vendorized/readme/__init__.py
--rw-r--r--   0        0        0       78 2021-05-09 15:40:19.105348 flit-3.8.0/flit/vendorized/readme/clean.py
--rw-r--r--   0        0        0     4180 2021-11-14 14:34:30.346272 flit-3.8.0/flit/vendorized/readme/rst.py
--rw-r--r--   0        0        0      280 2021-11-14 14:34:30.346272 flit-3.8.0/flit/wheel.py
--rw-r--r--   0        0        0     1525 2022-11-05 12:52:43.629104 flit-3.8.0/flit_core/LICENSE
--rw-r--r--   0        0        0      171 2021-11-14 14:34:30.346272 flit-3.8.0/flit_core/README.rst
--rw-r--r--   0        0        0     1742 2022-11-05 12:52:43.629104 flit-3.8.0/flit_core/bootstrap_install.py
--rw-r--r--   0        0        0      421 2022-11-05 12:52:27.470017 flit-3.8.0/flit_core/build_dists.py
--rw-r--r--   0        0        0      224 2022-11-05 13:06:27.382138 flit-3.8.0/flit_core/flit_core/__init__.py
--rw-r--r--   0        0        0     3282 2021-11-14 14:34:30.346272 flit-3.8.0/flit_core/flit_core/buildapi.py
--rw-r--r--   0        0        0    14520 2022-11-05 12:52:43.629104 flit-3.8.0/flit_core/flit_core/common.py
--rw-r--r--   0        0        0    23247 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/config.py
--rw-r--r--   0        0        0     7045 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/sdist.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/__init__.py
--rw-r--r--   0        0        0      165 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/EG_README.rst
--rw-r--r--   0        0        0      221 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/bad-description-ext.toml
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/conflicting_modules/module1.py
--rw-r--r--   0        0        0      180 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/conflicting_modules/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/conflicting_modules/src/module1.py
--rw-r--r--   0        0        0      115 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/constructed_version/module1.py
--rw-r--r--   0        0        0      266 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/constructed_version/pyproject.toml
--rw-r--r--   0        0        0      305 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/extras-dev-conflict.toml
--rw-r--r--   0        0        0      361 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/extras.toml
--rw-r--r--   0        0        0      103 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/samples/imported_version/package1/__init__.py
--rw-r--r--   0        0        0       22 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/samples/imported_version/package1/_version.py
--rw-r--r--   0        0        0      220 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/samples/imported_version/pyproject.toml
--rw-r--r--   0        0        0      100 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/inclusion/LICENSES/README
--rw-r--r--   0        0        0        0 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/samples/inclusion/doc/subdir/subsubdir/test.md
--rw-r--r--   0        0        0       48 2021-11-14 14:34:30.347272 flit-3.8.0/flit_core/flit_core/tests/samples/inclusion/doc/subdir/test.txt
--rw-r--r--   0        0        0       48 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/inclusion/doc/test.rst
--rw-r--r--   0        0        0       48 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/inclusion/doc/test.txt
--rw-r--r--   0        0        0       37 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/inclusion/module1.py
--rw-r--r--   0        0        0      239 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/samples/inclusion/pyproject.toml
--rw-r--r--   0        0        0       95 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/invalid_version1.py
--rw-r--r--   0        0        0      254 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/missing-description-file.toml
--rw-r--r--   0        0        0      299 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/misspelled-key.toml
--rw-r--r--   0        0        0      118 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/module1-pkg.ini
--rw-r--r--   0        0        0      288 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/module1-pkg.toml
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/module1.py
--rw-r--r--   0        0        0      187 2021-12-06 14:34:44.137786 flit-3.8.0/flit_core/flit_core/tests/samples/module2.py
--rw-r--r--   0        0        0       80 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/moduleunimportable.py
--rw-r--r--   0        0        0      113 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/samples/moduleunimportabledouble.py
--rw-r--r--   0        0        0       29 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/my-description.rst
--rw-r--r--   0        0        0      303 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/no_docstring-pkg.toml
--rw-r--r--   0        0        0       20 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/no_docstring.py
--rw-r--r--   0        0        0        0 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/samples/normalization/my_python_module.py
--rw-r--r--   0        0        0      333 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/samples/normalization/pyproject.toml
--rw-r--r--   0        0        0      165 2021-11-18 22:10:43.577393 flit-3.8.0/flit_core/flit_core/tests/samples/ns1-pkg/EG_README.rst
--rw-r--r--   0        0        0       76 2021-11-18 22:10:43.577393 flit-3.8.0/flit_core/flit_core/tests/samples/ns1-pkg/ns1/pkg/__init__.py
--rw-r--r--   0        0        0      266 2021-11-18 22:10:43.577393 flit-3.8.0/flit_core/flit_core/tests/samples/ns1-pkg/pyproject.toml
--rw-r--r--   0        0        0      311 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/package1.toml
--rw-r--r--   0        0        0       84 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/package1/__init__.py
--rw-r--r--   0        0        0       35 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/package1/data_dir/foo.sh
--rw-r--r--   0        0        0        6 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/package1/foo.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/package1/subpkg/__init__.py
--rw-r--r--   0        0        0       18 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/package1/subpkg/sp_data_dir/test.json
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/package1/subpkg2/__init__.py
--rw-r--r--   0        0        0       36 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/pep517/LICENSE
--rw-r--r--   0        0        0       37 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/pep517/README.rst
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.348272 flit-3.8.0/flit_core/flit_core/tests/samples/pep517/module1.py
--rw-r--r--   0        0        0      380 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/pep517/pyproject.toml
--rw-r--r--   0        0        0       36 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/pep621/LICENSE
--rw-r--r--   0        0        0       37 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/pep621/README.rst
--rw-r--r--   0        0        0       42 2022-04-09 19:45:18.284031 flit-3.8.0/flit_core/flit_core/tests/samples/pep621/module1a.py
--rw-r--r--   0        0        0      694 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/pep621/pyproject.toml
--rw-r--r--   0        0        0       37 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/pep621_nodynamic/README.rst
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/pep621_nodynamic/module1.py
--rw-r--r--   0        0        0      650 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/pep621_nodynamic/pyproject.toml
--rw-r--r--   0        0        0      311 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/requires-dev.toml
--rw-r--r--   0        0        0      252 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/requires-envmark.toml
--rw-r--r--   0        0        0      299 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/requires-extra-envmark.toml
--rw-r--r--   0        0        0      239 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/samples/requires-requests.toml
--rw-r--r--   0        0        0       36 2022-11-05 12:52:27.545017 flit-3.8.0/flit_core/flit_core/tests/samples/with_data_dir/LICENSE
--rw-r--r--   0        0        0       37 2022-11-05 12:52:27.545017 flit-3.8.0/flit_core/flit_core/tests/samples/with_data_dir/README.rst
--rw-r--r--   0        0        0       18 2022-11-05 12:52:27.545017 flit-3.8.0/flit_core/flit_core/tests/samples/with_data_dir/data/share/man/man1/foo.1
--rw-r--r--   0        0        0       42 2022-11-05 12:52:27.545017 flit-3.8.0/flit_core/flit_core/tests/samples/with_data_dir/module1.py
--rw-r--r--   0        0        0      452 2022-11-05 12:52:27.545017 flit-3.8.0/flit_core/flit_core/tests/samples/with_data_dir/pyproject.toml
--rw-r--r--   0        0        0     1552 2022-11-05 12:52:27.470017 flit-3.8.0/flit_core/flit_core/tests/test_build_thyself.py
--rw-r--r--   0        0        0     3934 2021-11-14 14:34:30.349272 flit-3.8.0/flit_core/flit_core/tests/test_buildapi.py
--rw-r--r--   0        0        0     5951 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/test_common.py
--rw-r--r--   0        0        0     7316 2022-11-05 12:52:43.630104 flit-3.8.0/flit_core/flit_core/tests/test_config.py
--rw-r--r--   0        0        0     1941 2022-11-05 12:52:43.631104 flit-3.8.0/flit_core/flit_core/tests/test_sdist.py
--rw-r--r--   0        0        0     1170 2021-11-14 14:34:30.350272 flit-3.8.0/flit_core/flit_core/tests/test_versionno.py
--rw-r--r--   0        0        0     1716 2022-11-05 12:52:43.631104 flit-3.8.0/flit_core/flit_core/tests/test_wheel.py
--rw-r--r--   0        0        0      791 2022-11-05 12:52:27.463017 flit-3.8.0/flit_core/flit_core/vendor/README
--rw-r--r--   0        0        0        0 2022-11-05 12:52:27.447017 flit-3.8.0/flit_core/flit_core/vendor/__init__.py
--rw-r--r--   0        0        0     1072 2022-11-05 12:52:27.452017 flit-3.8.0/flit_core/flit_core/vendor/tomli-1.2.3.dist-info/LICENSE
--rw-r--r--   0        0        0     9089 2022-11-05 12:52:27.452017 flit-3.8.0/flit_core/flit_core/vendor/tomli-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      294 2022-11-05 12:52:27.452017 flit-3.8.0/flit_core/flit_core/vendor/tomli/__init__.py
--rw-r--r--   0        0        0    21649 2022-11-05 12:52:27.452017 flit-3.8.0/flit_core/flit_core/vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2813 2022-11-05 12:52:27.452017 flit-3.8.0/flit_core/flit_core/vendor/tomli/_re.py
--rw-r--r--   0        0        0      126 2022-11-05 12:52:27.452017 flit-3.8.0/flit_core/flit_core/vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2022-11-05 12:52:27.452017 flit-3.8.0/flit_core/flit_core/vendor/tomli/py.typed
--rw-r--r--   0        0        0     4781 2021-11-14 14:34:30.350272 flit-3.8.0/flit_core/flit_core/versionno.py
--rw-r--r--   0        0        0     9269 2022-11-05 12:52:43.631104 flit-3.8.0/flit_core/flit_core/wheel.py
--rw-r--r--   0        0        0      651 2022-11-05 12:52:43.631104 flit-3.8.0/flit_core/pyproject.toml
--rwxr-xr-x   0        0        0      555 2022-11-05 12:52:27.447017 flit-3.8.0/flit_core/update-vendored-tomli.sh
--rw-r--r--   0        0        0     1007 2022-11-05 13:06:27.381138 flit-3.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-05-09 15:40:19.109348 flit-3.8.0/tests/__init__.py
--rw-r--r--   0        0        0      372 2021-11-14 14:34:30.350272 flit-3.8.0/tests/conftest.py
--rw-r--r--   0        0        0      165 2021-05-09 15:40:19.109348 flit-3.8.0/tests/samples/EG_README.rst
--rw-r--r--   0        0        0       84 2021-11-14 14:34:30.350272 flit-3.8.0/tests/samples/altdistname/package1/__init__.py
--rw-r--r--   0        0        0       35 2021-11-14 14:34:30.350272 flit-3.8.0/tests/samples/altdistname/package1/data_dir/foo.sh
--rw-r--r--   0        0        0        6 2021-11-14 14:34:30.350272 flit-3.8.0/tests/samples/altdistname/package1/foo.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.350272 flit-3.8.0/tests/samples/altdistname/package1/subpkg/__init__.py
--rw-r--r--   0        0        0       18 2021-11-14 14:34:30.350272 flit-3.8.0/tests/samples/altdistname/package1/subpkg/sp_data_dir/test.json
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/altdistname/package1/subpkg2/__init__.py
--rw-r--r--   0        0        0      260 2022-11-05 12:52:27.507017 flit-3.8.0/tests/samples/altdistname/pyproject.toml
--rw-r--r--   0        0        0      221 2021-05-09 15:40:19.110348 flit-3.8.0/tests/samples/bad-description-ext.toml
--rw-r--r--   0        0        0       29 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_conflict/console_entry_points.txt
--rw-r--r--   0        0        0       84 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_conflict/package1/__init__.py
--rw-r--r--   0        0        0       35 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_conflict/package1/data_dir/foo.sh
--rw-r--r--   0        0        0        6 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_conflict/package1/foo.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_conflict/package1/subpkg/__init__.py
--rw-r--r--   0        0        0       18 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_conflict/package1/subpkg/sp_data_dir/test.json
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_conflict/package1/subpkg2/__init__.py
--rw-r--r--   0        0        0      368 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_conflict/pyproject.toml
--rw-r--r--   0        0        0       84 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_valid/package1/__init__.py
--rw-r--r--   0        0        0       35 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_valid/package1/data_dir/foo.sh
--rw-r--r--   0        0        0        6 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_valid/package1/foo.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_valid/package1/subpkg/__init__.py
--rw-r--r--   0        0        0       18 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_valid/package1/subpkg/sp_data_dir/test.json
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_valid/package1/subpkg2/__init__.py
--rw-r--r--   0        0        0      343 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/entrypoints_valid/pyproject.toml
--rw-r--r--   0        0        0      305 2021-05-09 15:40:19.111348 flit-3.8.0/tests/samples/extras-dev-conflict.toml
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/extras/module1.py
--rw-r--r--   0        0        0      277 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/extras/pyproject.toml
--rw-r--r--   0        0        0      370 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/invalid_classifier.toml
--rw-r--r--   0        0        0       95 2021-05-09 15:40:19.111348 flit-3.8.0/tests/samples/invalid_version1.py
--rw-r--r--   0        0        0      254 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/missing-description-file.toml
--rw-r--r--   0        0        0       42 2021-05-09 15:40:19.111348 flit-3.8.0/tests/samples/module1.py
--rw-r--r--   0        0        0      118 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/module1_ini/flit.ini
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.351272 flit-3.8.0/tests/samples/module1_ini/module1.py
--rw-r--r--   0        0        0      165 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/module1_toml/EG_README.rst
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/module1_toml/module1.py
--rw-r--r--   0        0        0      288 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/module1_toml/pyproject.toml
--rw-r--r--   0        0        0       60 2021-05-09 15:40:19.112348 flit-3.8.0/tests/samples/module2.py
--rw-r--r--   0        0        0       44 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/module3/LICENSE
--rw-r--r--   0        0        0      230 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/module3/pyproject.toml
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/module3/src/module3.py
--rw-r--r--   0        0        0       80 2021-05-09 15:40:19.112348 flit-3.8.0/tests/samples/moduleunimportable.py
--rw-r--r--   0        0        0      115 2021-05-09 15:40:19.112348 flit-3.8.0/tests/samples/modulewithconstructedversion.py
--rw-r--r--   0        0        0       79 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/modulewithlocalversion/modulewithlocalversion.py
--rw-r--r--   0        0        0      260 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/modulewithlocalversion/pyproject.toml
--rw-r--r--   0        0        0       29 2021-05-09 15:40:19.112348 flit-3.8.0/tests/samples/my-description.rst
--rw-r--r--   0        0        0      303 2021-05-09 15:40:19.112348 flit-3.8.0/tests/samples/no_docstring-pkg.toml
--rw-r--r--   0        0        0       20 2021-05-09 15:40:19.112348 flit-3.8.0/tests/samples/no_docstring.py
--rw-r--r--   0        0        0       82 2021-11-18 22:10:43.578393 flit-3.8.0/tests/samples/ns1-pkg-mod/ns1/module.py
--rw-r--r--   0        0        0      154 2021-11-18 22:10:43.578393 flit-3.8.0/tests/samples/ns1-pkg-mod/pyproject.toml
--rw-r--r--   0        0        0      165 2021-11-18 22:10:43.578393 flit-3.8.0/tests/samples/ns1-pkg/EG_README.rst
--rw-r--r--   0        0        0       76 2021-11-18 22:10:43.578393 flit-3.8.0/tests/samples/ns1-pkg/ns1/pkg/__init__.py
--rw-r--r--   0        0        0      266 2021-11-18 22:10:43.578393 flit-3.8.0/tests/samples/ns1-pkg/pyproject.toml
--rw-r--r--   0        0        0      165 2021-11-18 22:10:43.578393 flit-3.8.0/tests/samples/ns1-pkg2/EG_README.rst
--rw-r--r--   0        0        0       77 2021-11-18 22:10:43.578393 flit-3.8.0/tests/samples/ns1-pkg2/ns1/pkg2/__init__.py
--rw-r--r--   0        0        0      267 2021-11-18 22:10:43.579393 flit-3.8.0/tests/samples/ns1-pkg2/pyproject.toml
--rw-r--r--   0        0        0       29 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package1/my-description.rst
--rw-r--r--   0        0        0       84 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package1/package1/__init__.py
--rw-r--r--   0        0        0       35 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package1/package1/data_dir/foo.sh
--rw-r--r--   0        0        0        6 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package1/package1/foo.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package1/package1/subpkg/__init__.py
--rw-r--r--   0        0        0       18 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package1/package1/subpkg/sp_data_dir/test.json
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package1/package1/subpkg2/__init__.py
--rw-r--r--   0        0        0      321 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package1/pyproject.toml
--rw-r--r--   0        0        0      156 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package2/package2-pkg.ini
--rw-r--r--   0        0        0      271 2021-11-14 14:34:30.352272 flit-3.8.0/tests/samples/package2/pyproject.toml
--rw-r--r--   0        0        0       84 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/package2/src/package2/__init__.py
--rw-r--r--   0        0        0        6 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/package2/src/package2/foo.py
--rw-r--r--   0        0        0      226 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/packageinsrc/pyproject.toml
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/packageinsrc/src/module1.py
--rw-r--r--   0        0        0       42 2021-05-09 15:40:19.114348 flit-3.8.0/tests/samples/pep517/module1.py
--rw-r--r--   0        0        0      267 2021-05-09 15:40:19.114348 flit-3.8.0/tests/samples/pep517/pyproject.toml
--rw-r--r--   0        0        0      311 2021-05-09 15:40:19.114348 flit-3.8.0/tests/samples/requires-dev.toml
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/requires-envmark/module1.py
--rw-r--r--   0        0        0      252 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/requires-envmark/pyproject.toml
--rw-r--r--   0        0        0       42 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/requires-extra-envmark/module1.py
--rw-r--r--   0        0        0      264 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/requires-extra-envmark/pyproject.toml
--rw-r--r--   0        0        0      239 2021-05-09 15:40:19.114348 flit-3.8.0/tests/samples/requires-requests.toml
--rw-r--r--   0        0        0      196 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/with_flit_ini/flit.ini
--rw-r--r--   0        0        0       84 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/with_flit_ini/package1/__init__.py
--rw-r--r--   0        0        0        6 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/with_flit_ini/package1/foo.py
--rw-r--r--   0        0        0        0 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/with_flit_ini/package1/subpkg/__init__.py
--rw-r--r--   0        0        0       34 2021-11-14 14:34:30.353272 flit-3.8.0/tests/samples/with_flit_ini/some_entry_points.txt
--rw-r--r--   0        0        0     2932 2021-11-18 22:10:43.579393 flit-3.8.0/tests/test_build.py
--rw-r--r--   0        0        0      460 2022-11-05 12:25:12.655161 flit-3.8.0/tests/test_command.py
--rw-r--r--   0        0        0      278 2021-11-14 14:34:30.353272 flit-3.8.0/tests/test_config.py
--rw-r--r--   0        0        0      780 2021-11-14 14:34:30.353272 flit-3.8.0/tests/test_find_python_executable.py
--rw-r--r--   0        0        0     8350 2022-11-05 13:06:10.848055 flit-3.8.0/tests/test_init.py
--rw-r--r--   0        0        0    15543 2022-11-05 12:52:43.631104 flit-3.8.0/tests/test_install.py
--rw-r--r--   0        0        0     5433 2021-11-18 22:10:43.579393 flit-3.8.0/tests/test_sdist.py
--rw-r--r--   0        0        0      788 2022-11-05 12:52:43.631104 flit-3.8.0/tests/test_tomlify.py
--rw-r--r--   0        0        0     4517 2022-11-05 12:52:43.631104 flit-3.8.0/tests/test_upload.py
--rw-r--r--   0        0        0     7492 2021-12-06 14:34:44.138786 flit-3.8.0/tests/test_validate.py
--rw-r--r--   0        0        0      594 2021-05-09 15:40:19.115348 flit-3.8.0/tests/test_vcs.py
--rw-r--r--   0        0        0     8436 2021-11-18 22:10:43.579393 flit-3.8.0/tests/test_wheel.py
--rw-r--r--   0        0        0      831 2022-11-05 12:52:43.632104 flit-3.8.0/tox.ini
--rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 flit-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0      295 2023-05-14 14:47:29.186488 flit-3.9.0/.bumpversion.cfg
+-rw-r--r--   0        0        0       48 2023-05-14 14:43:38.918691 flit-3.9.0/.coveragerc
+-rw-r--r--   0        0        0      117 2023-05-14 14:43:38.918691 flit-3.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1445 2023-05-14 14:43:38.918691 flit-3.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      207 2021-11-18 22:10:43.574393 flit-3.9.0/.gitignore
+-rw-r--r--   0        0        0      166 2023-05-14 14:43:44.522708 flit-3.9.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1525 2021-05-09 15:40:19.101348 flit-3.9.0/LICENSE
+-rw-r--r--   0        0        0     2565 2022-11-05 12:27:30.176410 flit-3.9.0/README.rst
+-rw-r--r--   0        0        0     1044 2023-05-14 14:43:38.918691 flit-3.9.0/bootstrap_dev.py
+-rw-r--r--   0        0        0       13 2021-05-09 15:40:19.102348 flit-3.9.0/codecov.yml
+-rw-r--r--   0        0        0     6754 2021-05-09 15:40:19.102348 flit-3.9.0/doc/Makefile
+-rw-r--r--   0        0        0     8893 2021-05-09 15:40:19.102348 flit-3.9.0/doc/_static/flit_logo_nobg.svg
+-rw-r--r--   0        0        0     5890 2021-05-09 15:40:19.102348 flit-3.9.0/doc/_static/flit_logo_nobg_cropped.png
+-rw-r--r--   0        0        0     9141 2021-05-09 15:40:19.102348 flit-3.9.0/doc/_static/flit_logo_nobg_cropped.svg
+-rw-r--r--   0        0        0     1735 2023-05-14 14:43:38.918691 flit-3.9.0/doc/bootstrap.rst
+-rw-r--r--   0        0        0     8351 2023-05-14 14:43:44.525708 flit-3.9.0/doc/cmdline.rst
+-rw-r--r--   0        0        0     8306 2023-05-14 14:47:29.186488 flit-3.9.0/doc/conf.py
+-rw-r--r--   0        0        0      585 2023-05-14 14:43:38.922691 flit-3.9.0/doc/development.rst
+-rw-r--r--   0        0        0     3422 2021-12-06 14:34:44.136786 flit-3.9.0/doc/flit_ini.rst
+-rw-r--r--   0        0        0    22116 2023-05-14 14:43:44.526708 flit-3.9.0/doc/history.rst
+-rw-r--r--   0        0        0      451 2021-11-14 14:34:30.343272 flit-3.9.0/doc/index.rst
+-rw-r--r--   0        0        0     6697 2021-05-09 15:40:19.103348 flit-3.9.0/doc/make.bat
+-rw-r--r--   0        0        0    16480 2023-05-14 14:43:38.923691 flit-3.9.0/doc/pyproject_toml.rst
+-rw-r--r--   0        0        0     2829 2021-11-14 14:34:30.343272 flit-3.9.0/doc/rationale.rst
+-rw-r--r--   0        0        0     1396 2021-05-09 15:40:19.103348 flit-3.9.0/doc/reproducible.rst
+-rw-r--r--   0        0        0       70 2021-11-14 14:34:30.344272 flit-3.9.0/doc/requirements.txt
+-rw-r--r--   0        0        0     2853 2021-11-14 14:34:30.344272 flit-3.9.0/doc/upload.rst
+-rw-r--r--   0        0        0     8989 2023-05-14 14:47:29.185487 flit-3.9.0/flit/__init__.py
+-rw-r--r--   0        0        0       68 2021-05-09 15:40:19.103348 flit-3.9.0/flit/__main__.py
+-rw-r--r--   0        0        0      898 2021-05-09 15:40:19.103348 flit-3.9.0/flit/_get_dirs.py
+-rw-r--r--   0        0        0     2151 2023-05-14 14:43:38.924691 flit-3.9.0/flit/build.py
+-rw-r--r--   0        0        0       33 2021-11-14 14:34:30.344272 flit-3.9.0/flit/buildapi.py
+-rw-r--r--   0        0        0      592 2021-11-14 14:34:30.344272 flit-3.9.0/flit/config.py
+-rw-r--r--   0        0        0     9093 2021-11-14 14:34:30.344272 flit-3.9.0/flit/init.py
+-rw-r--r--   0        0        0    16799 2023-05-14 14:43:38.925691 flit-3.9.0/flit/install.py
+-rw-r--r--   0        0        0     9161 2021-05-09 15:40:19.104348 flit-3.9.0/flit/license_templates/apache
+-rw-r--r--   0        0        0    32422 2021-05-09 15:40:19.104348 flit-3.9.0/flit/license_templates/gpl3
+-rw-r--r--   0        0        0     1077 2021-05-09 15:40:19.104348 flit-3.9.0/flit/license_templates/mit
+-rw-r--r--   0        0        0     4048 2021-05-09 15:40:19.104348 flit-3.9.0/flit/log.py
+-rw-r--r--   0        0        0      468 2021-05-09 15:40:19.104348 flit-3.9.0/flit/logo.py
+-rw-r--r--   0        0        0     8313 2023-05-14 14:43:38.925691 flit-3.9.0/flit/sdist.py
+-rw-r--r--   0        0        0     2297 2021-11-14 14:34:30.345272 flit-3.9.0/flit/tomlify.py
+-rw-r--r--   0        0        0     9350 2023-05-14 14:43:38.926691 flit-3.9.0/flit/upload.py
+-rw-r--r--   0        0        0    10032 2021-11-14 14:34:30.345272 flit-3.9.0/flit/validate.py
+-rw-r--r--   0        0        0      314 2021-11-14 14:34:30.346272 flit-3.9.0/flit/vcs/__init__.py
+-rw-r--r--   0        0        0      574 2021-11-14 14:34:30.346272 flit-3.9.0/flit/vcs/git.py
+-rw-r--r--   0        0        0     1258 2023-05-14 14:43:38.926691 flit-3.9.0/flit/vcs/hg.py
+-rw-r--r--   0        0        0        0 2021-05-09 15:40:19.104348 flit-3.9.0/flit/vendorized/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-09 15:40:19.105348 flit-3.9.0/flit/vendorized/readme/__init__.py
+-rw-r--r--   0        0        0       78 2021-05-09 15:40:19.105348 flit-3.9.0/flit/vendorized/readme/clean.py
+-rw-r--r--   0        0        0     4180 2021-11-14 14:34:30.346272 flit-3.9.0/flit/vendorized/readme/rst.py
+-rw-r--r--   0        0        0      280 2021-11-14 14:34:30.346272 flit-3.9.0/flit/wheel.py
+-rw-r--r--   0        0        0     1525 2023-05-14 14:43:38.926691 flit-3.9.0/flit_core/LICENSE
+-rw-r--r--   0        0        0      333 2023-05-14 14:43:38.926691 flit-3.9.0/flit_core/README.rst
+-rw-r--r--   0        0        0     1742 2023-05-14 14:43:38.926691 flit-3.9.0/flit_core/bootstrap_install.py
+-rw-r--r--   0        0        0      421 2023-05-14 14:43:38.926691 flit-3.9.0/flit_core/build_dists.py
+-rw-r--r--   0        0        0      224 2023-05-14 14:47:29.185487 flit-3.9.0/flit_core/flit_core/__init__.py
+-rw-r--r--   0        0        0     3282 2021-11-14 14:34:30.346272 flit-3.9.0/flit_core/flit_core/buildapi.py
+-rw-r--r--   0        0        0    15145 2023-05-14 14:43:38.927691 flit-3.9.0/flit_core/flit_core/common.py
+-rw-r--r--   0        0        0    23247 2023-05-14 14:43:38.927691 flit-3.9.0/flit_core/flit_core/config.py
+-rw-r--r--   0        0        0     7237 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/sdist.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/__init__.py
+-rw-r--r--   0        0        0      165 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/EG_README.rst
+-rw-r--r--   0        0        0      221 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/bad-description-ext.toml
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/conflicting_modules/module1.py
+-rw-r--r--   0        0        0      180 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/conflicting_modules/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/conflicting_modules/src/module1.py
+-rw-r--r--   0        0        0      115 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/constructed_version/module1.py
+-rw-r--r--   0        0        0      266 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/constructed_version/pyproject.toml
+-rw-r--r--   0        0        0      305 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/extras-dev-conflict.toml
+-rw-r--r--   0        0        0      361 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/extras.toml
+-rw-r--r--   0        0        0      138 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/tests/samples/imported_version/package1/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/tests/samples/imported_version/package1/_version.py
+-rw-r--r--   0        0        0      220 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/tests/samples/imported_version/pyproject.toml
+-rw-r--r--   0        0        0      100 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/inclusion/LICENSES/README
+-rw-r--r--   0        0        0        0 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/tests/samples/inclusion/doc/subdir/subsubdir/test.md
+-rw-r--r--   0        0        0       48 2021-11-14 14:34:30.347272 flit-3.9.0/flit_core/flit_core/tests/samples/inclusion/doc/subdir/test.txt
+-rw-r--r--   0        0        0       48 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/inclusion/doc/test.rst
+-rw-r--r--   0        0        0       48 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/inclusion/doc/test.txt
+-rw-r--r--   0        0        0       37 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/inclusion/module1.py
+-rw-r--r--   0        0        0      239 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/tests/samples/inclusion/pyproject.toml
+-rw-r--r--   0        0        0       95 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/invalid_version1.py
+-rw-r--r--   0        0        0      254 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/missing-description-file.toml
+-rw-r--r--   0        0        0      299 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/misspelled-key.toml
+-rw-r--r--   0        0        0      118 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/module1-pkg.ini
+-rw-r--r--   0        0        0      288 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/module1-pkg.toml
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/module1.py
+-rw-r--r--   0        0        0      187 2021-12-06 14:34:44.137786 flit-3.9.0/flit_core/flit_core/tests/samples/module2.py
+-rw-r--r--   0        0        0       80 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/moduleunimportable.py
+-rw-r--r--   0        0        0      113 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/tests/samples/moduleunimportabledouble.py
+-rw-r--r--   0        0        0       29 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/my-description.rst
+-rw-r--r--   0        0        0      303 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/no_docstring-pkg.toml
+-rw-r--r--   0        0        0       20 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/no_docstring.py
+-rw-r--r--   0        0        0        0 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/tests/samples/normalization/my_python_module.py
+-rw-r--r--   0        0        0      334 2023-05-14 14:43:38.928691 flit-3.9.0/flit_core/flit_core/tests/samples/normalization/pyproject.toml
+-rw-r--r--   0        0        0      165 2021-11-18 22:10:43.577393 flit-3.9.0/flit_core/flit_core/tests/samples/ns1-pkg/EG_README.rst
+-rw-r--r--   0        0        0       76 2021-11-18 22:10:43.577393 flit-3.9.0/flit_core/flit_core/tests/samples/ns1-pkg/ns1/pkg/__init__.py
+-rw-r--r--   0        0        0      266 2021-11-18 22:10:43.577393 flit-3.9.0/flit_core/flit_core/tests/samples/ns1-pkg/pyproject.toml
+-rw-r--r--   0        0        0      311 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/package1.toml
+-rw-r--r--   0        0        0       84 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/package1/__init__.py
+-rw-r--r--   0        0        0       35 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/package1/data_dir/foo.sh
+-rw-r--r--   0        0        0        6 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/package1/foo.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/package1/subpkg/__init__.py
+-rw-r--r--   0        0        0       18 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/package1/subpkg/sp_data_dir/test.json
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/package1/subpkg2/__init__.py
+-rw-r--r--   0        0        0       36 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/pep517/LICENSE
+-rw-r--r--   0        0        0       37 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/pep517/README.rst
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.348272 flit-3.9.0/flit_core/flit_core/tests/samples/pep517/module1.py
+-rw-r--r--   0        0        0      380 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/pep517/pyproject.toml
+-rw-r--r--   0        0        0       36 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/pep621/LICENSE
+-rw-r--r--   0        0        0       37 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/pep621/README.rst
+-rw-r--r--   0        0        0       42 2022-04-09 19:45:18.284031 flit-3.9.0/flit_core/flit_core/tests/samples/pep621/module1a.py
+-rw-r--r--   0        0        0      694 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/pep621/pyproject.toml
+-rw-r--r--   0        0        0       37 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/pep621_nodynamic/README.rst
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/pep621_nodynamic/module1.py
+-rw-r--r--   0        0        0      650 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/pep621_nodynamic/pyproject.toml
+-rw-r--r--   0        0        0      311 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/requires-dev.toml
+-rw-r--r--   0        0        0      252 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/requires-envmark.toml
+-rw-r--r--   0        0        0      299 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/requires-extra-envmark.toml
+-rw-r--r--   0        0        0      239 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/samples/requires-requests.toml
+-rw-r--r--   0        0        0       36 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/samples/with_data_dir/LICENSE
+-rw-r--r--   0        0        0       37 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/samples/with_data_dir/README.rst
+-rw-r--r--   0        0        0       18 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/samples/with_data_dir/data/share/man/man1/foo.1
+-rw-r--r--   0        0        0       42 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/samples/with_data_dir/module1.py
+-rw-r--r--   0        0        0      452 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/samples/with_data_dir/pyproject.toml
+-rw-r--r--   0        0        0     1552 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/test_build_thyself.py
+-rw-r--r--   0        0        0     3934 2021-11-14 14:34:30.349272 flit-3.9.0/flit_core/flit_core/tests/test_buildapi.py
+-rw-r--r--   0        0        0     5951 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/test_common.py
+-rw-r--r--   0        0        0     7316 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/test_config.py
+-rw-r--r--   0        0        0     2202 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/test_sdist.py
+-rw-r--r--   0        0        0     1170 2021-11-14 14:34:30.350272 flit-3.9.0/flit_core/flit_core/tests/test_versionno.py
+-rw-r--r--   0        0        0     1716 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/tests/test_wheel.py
+-rw-r--r--   0        0        0      791 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/vendor/README
+-rw-r--r--   0        0        0        0 2023-05-14 14:43:38.929691 flit-3.9.0/flit_core/flit_core/vendor/__init__.py
+-rw-r--r--   0        0        0     1072 2023-05-14 14:43:38.930691 flit-3.9.0/flit_core/flit_core/vendor/tomli-1.2.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     9089 2023-05-14 14:43:38.930691 flit-3.9.0/flit_core/flit_core/vendor/tomli-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      294 2023-05-14 14:43:38.930691 flit-3.9.0/flit_core/flit_core/vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    21649 2023-05-14 14:43:38.930691 flit-3.9.0/flit_core/flit_core/vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2813 2023-05-14 14:43:38.930691 flit-3.9.0/flit_core/flit_core/vendor/tomli/_re.py
+-rw-r--r--   0        0        0      126 2023-05-14 14:43:38.930691 flit-3.9.0/flit_core/flit_core/vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2023-05-14 14:43:38.930691 flit-3.9.0/flit_core/flit_core/vendor/tomli/py.typed
+-rw-r--r--   0        0        0     4781 2021-11-14 14:34:30.350272 flit-3.9.0/flit_core/flit_core/versionno.py
+-rw-r--r--   0        0        0     9306 2023-05-14 14:43:38.930691 flit-3.9.0/flit_core/flit_core/wheel.py
+-rw-r--r--   0        0        0      712 2023-05-14 14:43:38.931691 flit-3.9.0/flit_core/pyproject.toml
+-rwxr-xr-x   0        0        0      555 2023-05-14 14:43:38.931691 flit-3.9.0/flit_core/update-vendored-tomli.sh
+-rw-r--r--   0        0        0     1007 2023-05-14 14:47:29.184487 flit-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-05-09 15:40:19.109348 flit-3.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      372 2021-11-14 14:34:30.350272 flit-3.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      165 2021-05-09 15:40:19.109348 flit-3.9.0/tests/samples/EG_README.rst
+-rw-r--r--   0        0        0       84 2021-11-14 14:34:30.350272 flit-3.9.0/tests/samples/altdistname/package1/__init__.py
+-rw-r--r--   0        0        0       35 2021-11-14 14:34:30.350272 flit-3.9.0/tests/samples/altdistname/package1/data_dir/foo.sh
+-rw-r--r--   0        0        0        6 2021-11-14 14:34:30.350272 flit-3.9.0/tests/samples/altdistname/package1/foo.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.350272 flit-3.9.0/tests/samples/altdistname/package1/subpkg/__init__.py
+-rw-r--r--   0        0        0       18 2021-11-14 14:34:30.350272 flit-3.9.0/tests/samples/altdistname/package1/subpkg/sp_data_dir/test.json
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/altdistname/package1/subpkg2/__init__.py
+-rw-r--r--   0        0        0      260 2023-05-14 14:43:38.931691 flit-3.9.0/tests/samples/altdistname/pyproject.toml
+-rw-r--r--   0        0        0      221 2021-05-09 15:40:19.110348 flit-3.9.0/tests/samples/bad-description-ext.toml
+-rw-r--r--   0        0        0       29 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_conflict/console_entry_points.txt
+-rw-r--r--   0        0        0       84 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_conflict/package1/__init__.py
+-rw-r--r--   0        0        0       35 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_conflict/package1/data_dir/foo.sh
+-rw-r--r--   0        0        0        6 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_conflict/package1/foo.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_conflict/package1/subpkg/__init__.py
+-rw-r--r--   0        0        0       18 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_conflict/package1/subpkg/sp_data_dir/test.json
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_conflict/package1/subpkg2/__init__.py
+-rw-r--r--   0        0        0      368 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_conflict/pyproject.toml
+-rw-r--r--   0        0        0       84 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_valid/package1/__init__.py
+-rw-r--r--   0        0        0       35 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_valid/package1/data_dir/foo.sh
+-rw-r--r--   0        0        0        6 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_valid/package1/foo.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_valid/package1/subpkg/__init__.py
+-rw-r--r--   0        0        0       18 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_valid/package1/subpkg/sp_data_dir/test.json
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_valid/package1/subpkg2/__init__.py
+-rw-r--r--   0        0        0      343 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/entrypoints_valid/pyproject.toml
+-rw-r--r--   0        0        0      305 2021-05-09 15:40:19.111348 flit-3.9.0/tests/samples/extras-dev-conflict.toml
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/extras/module1.py
+-rw-r--r--   0        0        0      277 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/extras/pyproject.toml
+-rw-r--r--   0        0        0      370 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/invalid_classifier.toml
+-rw-r--r--   0        0        0       95 2021-05-09 15:40:19.111348 flit-3.9.0/tests/samples/invalid_version1.py
+-rw-r--r--   0        0        0      254 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/missing-description-file.toml
+-rw-r--r--   0        0        0       42 2021-05-09 15:40:19.111348 flit-3.9.0/tests/samples/module1.py
+-rw-r--r--   0        0        0      118 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/module1_ini/flit.ini
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.351272 flit-3.9.0/tests/samples/module1_ini/module1.py
+-rw-r--r--   0        0        0      165 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/module1_toml/EG_README.rst
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/module1_toml/module1.py
+-rw-r--r--   0        0        0      288 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/module1_toml/pyproject.toml
+-rw-r--r--   0        0        0       60 2021-05-09 15:40:19.112348 flit-3.9.0/tests/samples/module2.py
+-rw-r--r--   0        0        0       44 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/module3/LICENSE
+-rw-r--r--   0        0        0      230 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/module3/pyproject.toml
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/module3/src/module3.py
+-rw-r--r--   0        0        0       80 2021-05-09 15:40:19.112348 flit-3.9.0/tests/samples/moduleunimportable.py
+-rw-r--r--   0        0        0      115 2021-05-09 15:40:19.112348 flit-3.9.0/tests/samples/modulewithconstructedversion.py
+-rw-r--r--   0        0        0       79 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/modulewithlocalversion/modulewithlocalversion.py
+-rw-r--r--   0        0        0      260 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/modulewithlocalversion/pyproject.toml
+-rw-r--r--   0        0        0       29 2021-05-09 15:40:19.112348 flit-3.9.0/tests/samples/my-description.rst
+-rw-r--r--   0        0        0      303 2021-05-09 15:40:19.112348 flit-3.9.0/tests/samples/no_docstring-pkg.toml
+-rw-r--r--   0        0        0       20 2021-05-09 15:40:19.112348 flit-3.9.0/tests/samples/no_docstring.py
+-rw-r--r--   0        0        0       82 2021-11-18 22:10:43.578393 flit-3.9.0/tests/samples/ns1-pkg-mod/ns1/module.py
+-rw-r--r--   0        0        0      154 2021-11-18 22:10:43.578393 flit-3.9.0/tests/samples/ns1-pkg-mod/pyproject.toml
+-rw-r--r--   0        0        0      165 2021-11-18 22:10:43.578393 flit-3.9.0/tests/samples/ns1-pkg/EG_README.rst
+-rw-r--r--   0        0        0       76 2021-11-18 22:10:43.578393 flit-3.9.0/tests/samples/ns1-pkg/ns1/pkg/__init__.py
+-rw-r--r--   0        0        0      266 2021-11-18 22:10:43.578393 flit-3.9.0/tests/samples/ns1-pkg/pyproject.toml
+-rw-r--r--   0        0        0      165 2021-11-18 22:10:43.578393 flit-3.9.0/tests/samples/ns1-pkg2/EG_README.rst
+-rw-r--r--   0        0        0       77 2021-11-18 22:10:43.578393 flit-3.9.0/tests/samples/ns1-pkg2/ns1/pkg2/__init__.py
+-rw-r--r--   0        0        0      267 2021-11-18 22:10:43.579393 flit-3.9.0/tests/samples/ns1-pkg2/pyproject.toml
+-rw-r--r--   0        0        0       29 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package1/my-description.rst
+-rw-r--r--   0        0        0       84 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package1/package1/__init__.py
+-rw-r--r--   0        0        0       35 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package1/package1/data_dir/foo.sh
+-rw-r--r--   0        0        0        6 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package1/package1/foo.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package1/package1/subpkg/__init__.py
+-rw-r--r--   0        0        0       18 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package1/package1/subpkg/sp_data_dir/test.json
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package1/package1/subpkg2/__init__.py
+-rw-r--r--   0        0        0      321 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package1/pyproject.toml
+-rw-r--r--   0        0        0      156 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package2/package2-pkg.ini
+-rw-r--r--   0        0        0      271 2021-11-14 14:34:30.352272 flit-3.9.0/tests/samples/package2/pyproject.toml
+-rw-r--r--   0        0        0       84 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/package2/src/package2/__init__.py
+-rw-r--r--   0        0        0        6 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/package2/src/package2/foo.py
+-rw-r--r--   0        0        0      226 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/packageinsrc/pyproject.toml
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/packageinsrc/src/module1.py
+-rw-r--r--   0        0        0       42 2021-05-09 15:40:19.114348 flit-3.9.0/tests/samples/pep517/module1.py
+-rw-r--r--   0        0        0      267 2021-05-09 15:40:19.114348 flit-3.9.0/tests/samples/pep517/pyproject.toml
+-rw-r--r--   0        0        0      311 2021-05-09 15:40:19.114348 flit-3.9.0/tests/samples/requires-dev.toml
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/requires-envmark/module1.py
+-rw-r--r--   0        0        0      252 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/requires-envmark/pyproject.toml
+-rw-r--r--   0        0        0       42 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/requires-extra-envmark/module1.py
+-rw-r--r--   0        0        0      264 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/requires-extra-envmark/pyproject.toml
+-rw-r--r--   0        0        0      239 2021-05-09 15:40:19.114348 flit-3.9.0/tests/samples/requires-requests.toml
+-rw-r--r--   0        0        0      196 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/with_flit_ini/flit.ini
+-rw-r--r--   0        0        0       84 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/with_flit_ini/package1/__init__.py
+-rw-r--r--   0        0        0        6 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/with_flit_ini/package1/foo.py
+-rw-r--r--   0        0        0        0 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/with_flit_ini/package1/subpkg/__init__.py
+-rw-r--r--   0        0        0       34 2021-11-14 14:34:30.353272 flit-3.9.0/tests/samples/with_flit_ini/some_entry_points.txt
+-rw-r--r--   0        0        0     2932 2021-11-18 22:10:43.579393 flit-3.9.0/tests/test_build.py
+-rw-r--r--   0        0        0      460 2022-11-05 12:25:12.655161 flit-3.9.0/tests/test_command.py
+-rw-r--r--   0        0        0      278 2021-11-14 14:34:30.353272 flit-3.9.0/tests/test_config.py
+-rw-r--r--   0        0        0      780 2021-11-14 14:34:30.353272 flit-3.9.0/tests/test_find_python_executable.py
+-rw-r--r--   0        0        0     8350 2023-05-14 14:43:38.931691 flit-3.9.0/tests/test_init.py
+-rw-r--r--   0        0        0    15543 2023-05-14 14:43:38.931691 flit-3.9.0/tests/test_install.py
+-rw-r--r--   0        0        0     5433 2021-11-18 22:10:43.579393 flit-3.9.0/tests/test_sdist.py
+-rw-r--r--   0        0        0      788 2023-05-14 14:43:38.931691 flit-3.9.0/tests/test_tomlify.py
+-rw-r--r--   0        0        0     4517 2023-05-14 14:43:38.931691 flit-3.9.0/tests/test_upload.py
+-rw-r--r--   0        0        0     7492 2021-12-06 14:34:44.138786 flit-3.9.0/tests/test_validate.py
+-rw-r--r--   0        0        0      594 2021-05-09 15:40:19.115348 flit-3.9.0/tests/test_vcs.py
+-rw-r--r--   0        0        0     8586 2023-05-14 14:43:38.932691 flit-3.9.0/tests/test_wheel.py
+-rw-r--r--   0        0        0      831 2023-05-14 14:43:38.932691 flit-3.9.0/tox.ini
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 flit-3.9.0/PKG-INFO
```

### Comparing `flit-3.8.0/.github/workflows/test.yml` & `flit-3.9.0/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,39 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: ["ubuntu-latest", "windows-latest"]
-        python-version: [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11-dev" ]
+        python-version: [ "3.7", "3.8", "3.9", "3.10", "3.11" , "3.12-dev" ]
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Setup Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install tox tox-gh-actions codecov
+
+      - name: Run tests
+        run: tox
+
+      - name: Codecov upload
+        run: codecov
+
+  test-py36:
+    runs-on: "ubuntu-20.04"
+    strategy:
+      matrix:
+        python-version: [ "3.6", ]
     steps:
       - uses: actions/checkout@v3
 
       - name: Setup Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `flit-3.8.0/LICENSE` & `flit-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/README.rst` & `flit-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/bootstrap_dev.py` & `flit-3.9.0/bootstrap_dev.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/Makefile` & `flit-3.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/_static/flit_logo_nobg.svg` & `flit-3.9.0/doc/_static/flit_logo_nobg.svg`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/_static/flit_logo_nobg_cropped.png` & `flit-3.9.0/doc/_static/flit_logo_nobg_cropped.png`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/_static/flit_logo_nobg_cropped.svg` & `flit-3.9.0/doc/_static/flit_logo_nobg_cropped.svg`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/bootstrap.rst` & `flit-3.9.0/doc/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/cmdline.rst` & `flit-3.9.0/doc/cmdline.rst`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,32 @@
    An sdist built without this will only work with tools that support PEP 517,
    but the wheel will still be usable by any compatible tool.
 
    .. versionchanged:: 3.5
 
       Generating ``setup.py`` disabled by default.
 
+.. option:: --use-vcs
+
+   Use the files checked in to git or mercurial as the starting list to include
+   in an sdist, and then apply inclusions and exclusions :ref:`from pyproject.toml
+   <pyproject_toml_sdist>`.
+
+   This is the default for now, but we're planning to switch to ``--no-use-vcs``
+   as the default in a future version.
+
+.. option:: --no-use-vcs
+
+   Create the sdist starting with only the files inside the installed module
+   or package, along with any inclusions and exclusions defined in pyproject.toml.
+
+   With this option, sdists from ``flit build`` are equivalent to those built
+   by tools calling Flit as a backend, such as `build
+   <https://pypa-build.readthedocs.io/en/stable/>`_.
+
 .. _publish_cmd:
 
 ``flit publish``
 ----------------
 
 .. program:: flit publish
 
@@ -66,27 +84,20 @@
 
 .. option:: --format <format>
 
    Limit to publishing either ``wheel`` or ``sdist``.
    You should normally publish the two formats together.
 
 .. option:: --setup-py
-
-   Generate a ``setup.py`` file in the sdist, so it can be installed by older
-   versions of pip.
-
 .. option:: --no-setup-py
+.. option:: --use-vcs
+.. option:: --no-use-vcs
 
-   Don't generate a setup.py file in the sdist. This is the default.
-   An sdist built without this will only work with tools that support PEP 517,
-   but the wheel will still be usable by any compatible tool.
-
-   .. versionchanged:: 3.5
-
-      Generating ``setup.py`` disabled by default.
+   These options affecting what goes in the sdist are described for
+   :ref:`build_cmd` above.
 
 .. option:: --repository <repository>
 
    Name of a repository to upload packages to. Should match a section in
    ``~/.pypirc``. The default is ``pypi``.
 
 .. option:: --pypirc <pypirc>
```

### Comparing `flit-3.8.0/doc/conf.py` & `flit-3.9.0/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 copyright = u'2015, Thomas Kluyver'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '3.8.0'
+version = '3.9.0'
 # The full version, including alpha/beta/rc tags.
 release = version #+ '.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `flit-3.8.0/doc/development.rst` & `flit-3.9.0/doc/development.rst`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/flit_ini.rst` & `flit-3.9.0/doc/flit_ini.rst`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/history.rst` & `flit-3.9.0/doc/history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 Release history
 ===============
 
+Version 3.9
+-----------
+
+- New options :option:`flit build --use-vcs` and :option:`flit build --no-use-vcs`
+  to enable & disable including all committed files in the sdist. For now
+  ``--use-vcs`` is the default, but this is likely to change in a future
+  version, to bring ``flit build`` in line with standard build frontends like
+  ``python -m build`` (:ghpull:`625`).
+- Sdist file names, and the name of the top-level folder in an sdist, are now
+  normalised, in accordance with :pep:`625` (:ghpull:`628`).
+- A statically defined version number can now be parsed from files called
+  ``version.py``, ``_version.py`` or ``__version__.py`` inside a packge, as well
+  as from ``__init__.py``, so executing code is required in fewer cases
+  (:ghpull:`630`).
+- Fix setting the flag for regular files in zip metadata (:ghpull:`639`).
+- The timestamp embedded in the gzip wrapper for sdists now defaults to a fixed
+  date, so building an sdist twice on the same machine should produce identical
+  results, even without any special steps (:ghpull:`635`). Setting
+  :envvar:`SOURCE_DATE_EPOCH` is still recommended for properly
+  :doc:`reproducible builds <reproducible>`.
+
 Version 3.8
 -----------
 
 - A project name containing hyphens is now automatically translated to use
   underscores for the import name (:ghpull:`566`).
 - New option :option:`flit install --only-deps` to install the dependencies of
   the package, but not the package itself.
```

### Comparing `flit-3.8.0/doc/make.bat` & `flit-3.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/pyproject_toml.rst` & `flit-3.9.0/doc/pyproject_toml.rst`

 * *Files 3% similar despite different names*

```diff
@@ -396,18 +396,21 @@
 .. _pyproject_toml_sdist:
 
 Sdist section
 -------------
 
 .. versionadded:: 2.0
 
-When you use :ref:`build_cmd` or :ref:`publish_cmd`, Flit builds an sdist
-(source distribution) tarball containing the files that are checked into version
-control (git or mercurial). If you want more control, or it doesn't recognise
-your version control system, you can give lists of paths or glob patterns as
+With no configuration, Flit can make an sdist with everything it needs
+to build and install your module: the package contents (including non-Python
+data files, but not ``.pyc`` bytecode files), your ``pyproject.toml`` file,
+the readme & license files given in the metadata, and the :ref:`external data
+folder <pyproject_toml_external_data>` if you specified that.
+
+If you want more control, you can give lists of paths or glob patterns as
 ``include`` and ``exclude`` in this section. For example:
 
 .. code-block:: toml
 
     [tool.flit.sdist]
     include = ["doc/"]
     exclude = ["doc/*.html"]
@@ -425,21 +428,30 @@
 
 .. versionchanged:: 3.8
    Include and exclude patterns can now use recursive glob patterns (``**``).
 
 Exclusions have priority over inclusions. Bytecode is excluded by default and cannot
 be included.
 
-.. note::
+Including files committed in git/hg
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-   If you are not using :ref:`build_cmd` but  ``flit_core`` via another build
-   frontend, Flit doesn't doesn't check the VCS for files to include but instead
-   builds a 'minimal' sdist (which includes the files necessary to build a wheel).
-   You'll have to adapt your inclusion/exclusion rules to achieve the same result
-   as you'd get with :ref:`build_cmd`.
+If you use :ref:`build_cmd` or :ref:`publish_cmd`, you can also make sdists with
+the files which are committed in version control (git or hg). This is a shortcut
+to e.g. include documentation source files, but not built HTML or PDF
+documentation. The include and exclude patterns are then applied on top of this
+list.
+
+For now, including files from version control is the default for :ref:`build_cmd`
+and :ref:`publish_cmd`, and can be disabled with ``--no-use-vcs``. The default
+will switch in a future version.
+
+Using ``flit_core`` as a backend to other tools such as `build
+<https://pypa-build.readthedocs.io/en/latest/>`_ never gets the list of files
+for the sdist from version control.
 
 .. _pyproject_toml_external_data:
 
 External data section
 ---------------------
 
 .. versionadded:: 3.7
```

### Comparing `flit-3.8.0/doc/rationale.rst` & `flit-3.9.0/doc/rationale.rst`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/reproducible.rst` & `flit-3.9.0/doc/reproducible.rst`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/doc/upload.rst` & `flit-3.9.0/doc/upload.rst`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/__init__.py` & `flit-3.9.0/flit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 from typing import Optional
 
 from flit_core import common
 from .config import ConfigError
 from .log import enable_colourful_output
 
-__version__ = '3.8.0'
+__version__ = '3.9.0'
 
 log = logging.getLogger(__name__)
 
 
 class PythonNotFoundError(FileNotFoundError): pass
 
 
@@ -63,15 +63,55 @@
     parser.add_argument('--only-deps', action='store_true',
         help="Install only dependencies of this package, and not the package itself"
     )
     parser.add_argument('--extras', default=(), type=lambda l: l.split(',') if l else (),
         help="Install the dependencies of these (comma separated) extras additionally to the ones implied by --deps. "
              "--extras=all can be useful in combination with --deps=production, --deps=none precludes using --extras"
     )
-    
+
+
+def add_shared_build_options(parser: argparse.ArgumentParser):
+    parser.add_argument('--format', action='append',
+        help="Select a format to publish. Options: 'wheel', 'sdist'"
+    )
+
+    setup_py_grp = parser.add_mutually_exclusive_group()
+
+    setup_py_grp.add_argument('--setup-py', action='store_true',
+        help=("Generate a setup.py file in the sdist. "
+              "The sdist will work with older tools that predate PEP 517. "
+            )
+    )
+
+    setup_py_grp.add_argument('--no-setup-py', action='store_true',
+        help=("Don't generate a setup.py file in the sdist. This is the default. "
+              "The sdist will only work with tools that support PEP 517, "
+              "but the wheel will still be usable by any compatible tool."
+             )
+    )
+
+    vcs_grp = parser.add_mutually_exclusive_group()
+
+    vcs_grp.add_argument('--use-vcs', action='store_true',
+        help=("Choose which files to include in the sdist using git or hg. "
+              "This is a convenient way to include all checked-in files, like "
+              "tests and doc source files, in your sdist, but requires that git "
+              "or hg is available on the command line. This is currently the "
+              "default, but it will change in a future version. "
+             )
+    )
+
+    vcs_grp.add_argument('--no-use-vcs', action='store_true',
+        help=("Select the files to include in the sdist without using git or hg. "
+              "This should include all essential files to install and use your "
+              "package; see the documentation for precisely what is included. "
+              "This will become the default in a future version."
+             )
+    )
+
 
 def main(argv=None):
     ap = argparse.ArgumentParser()
     ap.add_argument('-f', '--ini-file', type=pathlib.Path, default='pyproject.toml')
     ap.add_argument('-V', '--version', action='version', version='Flit '+__version__)
     # --repository now belongs on 'flit publish' - it's still here for
     # compatibility with scripts passing it before the subcommand.
@@ -81,53 +121,22 @@
     subparsers = ap.add_subparsers(title='subcommands', dest='subcmd')
 
     # flit build --------------------------------------------
     parser_build = subparsers.add_parser('build',
         help="Build wheel and sdist",
     )
 
-    parser_build.add_argument('--format', action='append',
-        help="Select a format to build. Options: 'wheel', 'sdist'"
-    )
-
-    parser_build.add_argument('--setup-py', action='store_true',
-        help=("Generate a setup.py file in the sdist. "
-              "The sdist will work with older tools that predate PEP 517. "
-              )
-    )
-
-    parser_build.add_argument('--no-setup-py', action='store_true',
-        help=("Don't generate a setup.py file in the sdist. This is the default. "
-              "The sdist will only work with tools that support PEP 517, "
-              "but the wheel will still be usable by any compatible tool."
-             )
-    )
+    add_shared_build_options(parser_build)
 
     # flit publish --------------------------------------------
     parser_publish = subparsers.add_parser('publish',
         help="Upload wheel and sdist",
     )
 
-    parser_publish.add_argument('--format', action='append',
-        help="Select a format to publish. Options: 'wheel', 'sdist'"
-    )
-
-    parser_publish.add_argument('--setup-py', action='store_true',
-        help=("Generate a setup.py file in the sdist. "
-              "The sdist will work with older tools that predate PEP 517. "
-              "This is the default for now, but will change in a future version."
-              )
-    )
-
-    parser_publish.add_argument('--no-setup-py', action='store_true',
-        help=("Don't generate a setup.py file in the sdist. "
-              "The sdist will only work with tools that support PEP 517, "
-              "but the wheel will still be usable by any compatible tool."
-             )
-    )
+    add_shared_build_options(parser_publish)
 
     parser_publish.add_argument('--pypirc',
         help="The .pypirc config file to be used. DEFAULT = \"~/.pypirc\""
     )
 
     parser_publish.add_argument('--repository',
         help="Name of the repository to upload to (must be in the specified .pypirc file)"
@@ -169,28 +178,31 @@
         sys.exit(0)
 
     def gen_setup_py():
         if not (args.setup_py or args.no_setup_py):
             return False
         return args.setup_py
 
+    def sdist_use_vcs():
+        return not args.no_use_vcs
+
     if args.subcmd == 'build':
         from .build import main
         try:
             main(args.ini_file, formats=set(args.format or []),
-                 gen_setup_py=gen_setup_py())
+                 gen_setup_py=gen_setup_py(), use_vcs=sdist_use_vcs())
         except(common.NoDocstringError, common.VCSError, common.NoVersionError) as e:
             sys.exit(e.args[0])
     elif args.subcmd == 'publish':
         if args.deprecated_repository:
             log.warning("Passing --repository before the 'upload' subcommand is deprecated: pass it after")
         repository = args.repository or args.deprecated_repository
         from .upload import main
         main(args.ini_file, repository, args.pypirc, formats=set(args.format or []),
-                gen_setup_py=gen_setup_py())
+                gen_setup_py=gen_setup_py(), use_vcs=sdist_use_vcs())
 
     elif args.subcmd == 'install':
         from .install import Installer
         try:
             python = find_python_executable(args.python)
             installer = Installer.from_ini_path(
                 args.ini_file,
```

### Comparing `flit-3.8.0/flit/_get_dirs.py` & `flit-3.9.0/flit/_get_dirs.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/build.py` & `flit-3.9.0/flit/build.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     tf = tarfile.open(str(path))
     with TemporaryDirectory() as tmpdir:
         tf.extractall(tmpdir)
         files = os.listdir(tmpdir)
         assert len(files) == 1, files
         yield os.path.join(tmpdir, files[0])
 
-def main(ini_file: Path, formats=None, gen_setup_py=True):
+def main(ini_file: Path, formats=None, gen_setup_py=True, use_vcs=True):
     """Build wheel and sdist"""
     if not formats:
         formats = ALL_FORMATS
     elif not formats.issubset(ALL_FORMATS):
         raise ValueError("Unknown package formats: {}".format(formats - ALL_FORMATS))
 
     sdist_info = wheel_info = None
@@ -38,15 +38,15 @@
     dist_dir.mkdir(parents=True, exist_ok=True)
 
     try:
         # Load the config file to make sure it gets validated
         read_flit_config(ini_file)
 
         if 'sdist' in formats:
-            sb = SdistBuilder.from_ini_path(ini_file)
+            sb = SdistBuilder.from_ini_path(ini_file, use_vcs=use_vcs)
             sdist_file = sb.build(dist_dir, gen_setup_py=gen_setup_py)
             sdist_info = SimpleNamespace(builder=sb, file=sdist_file)
             # When we're building both, build the wheel from the unpacked sdist.
             # This helps ensure that the sdist contains all the necessary files.
             if 'wheel' in formats:
                 with unpacked_tarball(sdist_file) as tmpdir:
                     log.debug('Building wheel from unpacked sdist %s', tmpdir)
```

### Comparing `flit-3.8.0/flit/config.py` & `flit-3.9.0/flit/config.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/init.py` & `flit-3.9.0/flit/init.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/install.py` & `flit-3.9.0/flit/install.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/license_templates/apache` & `flit-3.9.0/flit/license_templates/apache`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/license_templates/gpl3` & `flit-3.9.0/flit/license_templates/gpl3`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/license_templates/mit` & `flit-3.9.0/flit/license_templates/mit`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/log.py` & `flit-3.9.0/flit/log.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/sdist.py` & `flit-3.9.0/flit/sdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,26 @@
     This extends the minimal sdist-building in flit_core:
 
     - Include any files tracked in version control, such as docs sources and
       tests.
     - Add a generated setup.py for compatibility with tools which don't yet know
       about PEP 517.
     """
+    use_vcs = True
+
+    @classmethod
+    def from_ini_path(cls, ini_path: Path, use_vcs=True):
+        inst = super().from_ini_path(ini_path)
+        inst.use_vcs = use_vcs
+        return inst
+
     def select_files(self):
+        if not self.use_vcs:
+            return super().select_files()
+
         vcs_mod = identify_vcs(self.cfgdir)
         if vcs_mod is not None:
             untracked_deleted = vcs_mod.list_untracked_deleted_files(self.cfgdir)
             if any(include_path(p) and not self.excludes.match_file(p)
                    for p in untracked_deleted):
                 raise VCSError(
                     "Untracked or deleted files in the source directory. "
```

### Comparing `flit-3.8.0/flit/tomlify.py` & `flit-3.9.0/flit/tomlify.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/upload.py` & `flit-3.9.0/flit/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,21 +256,24 @@
         if domain.startswith('upload.'):
             domain = domain[7:]
         log.info("Package is at https://%s/project/%s/", domain, metadata.name)
     else:
         log.info("Package is at %s/%s", repo['url'], metadata.name)
 
 
-def main(ini_path, repo_name, pypirc_path=None, formats=None, gen_setup_py=True):
+def main(ini_path, repo_name, pypirc_path=None, formats=None, gen_setup_py=True,
+         use_vcs=True):
     """Build and upload wheel and sdist."""
     if pypirc_path is None:
         pypirc_path = PYPIRC_DEFAULT
     elif not os.path.isfile(pypirc_path):
         raise FileNotFoundError("The specified pypirc config file does not exist.")
 
     from . import build
-    built = build.main(ini_path, formats=formats, gen_setup_py=gen_setup_py)
+    built = build.main(
+        ini_path, formats=formats, gen_setup_py=gen_setup_py, use_vcs=use_vcs
+    )
 
     if built.wheel is not None:
         do_upload(built.wheel.file, built.wheel.builder.metadata, pypirc_path, repo_name)
     if built.sdist is not None:
         do_upload(built.sdist.file, built.sdist.builder.metadata, pypirc_path, repo_name)
```

### Comparing `flit-3.8.0/flit/validate.py` & `flit-3.9.0/flit/validate.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/vcs/git.py` & `flit-3.9.0/flit/vcs/git.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/vcs/hg.py` & `flit-3.9.0/flit/vcs/hg.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit/vendorized/readme/rst.py` & `flit-3.9.0/flit/vendorized/readme/rst.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/LICENSE` & `flit-3.9.0/flit_core/LICENSE`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/bootstrap_install.py` & `flit-3.9.0/flit_core/bootstrap_install.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/buildapi.py` & `flit-3.9.0/flit_core/flit_core/buildapi.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/common.py` & `flit-3.9.0/flit_core/flit_core/common.py`

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

### Comparing `flit-3.8.0/flit_core/flit_core/config.py` & `flit-3.9.0/flit_core/flit_core/config.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/sdist.py` & `flit-3.9.0/flit_core/flit_core/sdist.py`

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

### Comparing `flit-3.8.0/flit_core/flit_core/tests/samples/pep621/pyproject.toml` & `flit-3.9.0/flit_core/flit_core/tests/samples/pep621/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/tests/samples/pep621_nodynamic/pyproject.toml` & `flit-3.9.0/flit_core/flit_core/tests/samples/pep621_nodynamic/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/tests/test_build_thyself.py` & `flit-3.9.0/flit_core/flit_core/tests/test_build_thyself.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/tests/test_buildapi.py` & `flit-3.9.0/flit_core/flit_core/tests/test_buildapi.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/tests/test_common.py` & `flit-3.9.0/flit_core/flit_core/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/tests/test_config.py` & `flit-3.9.0/flit_core/flit_core/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/tests/test_sdist.py` & `flit-3.9.0/flit_core/flit_core/tests/test_sdist.py`

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

### Comparing `flit-3.8.0/flit_core/flit_core/tests/test_versionno.py` & `flit-3.9.0/flit_core/flit_core/tests/test_versionno.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/tests/test_wheel.py` & `flit-3.9.0/flit_core/flit_core/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/vendor/README` & `flit-3.9.0/flit_core/flit_core/vendor/README`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/vendor/tomli-1.2.3.dist-info/LICENSE` & `flit-3.9.0/flit_core/flit_core/vendor/tomli-1.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/vendor/tomli-1.2.3.dist-info/METADATA` & `flit-3.9.0/flit_core/flit_core/vendor/tomli-1.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/vendor/tomli/_parser.py` & `flit-3.9.0/flit_core/flit_core/vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/vendor/tomli/_re.py` & `flit-3.9.0/flit_core/flit_core/vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/versionno.py` & `flit-3.9.0/flit_core/flit_core/versionno.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/flit_core/flit_core/wheel.py` & `flit-3.9.0/flit_core/flit_core/wheel.py`

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

### Comparing `flit-3.8.0/flit_core/pyproject.toml` & `flit-3.9.0/flit_core/pyproject.toml`

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

### Comparing `flit-3.8.0/flit_core/update-vendored-tomli.sh` & `flit-3.9.0/flit_core/update-vendored-tomli.sh`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/pyproject.toml` & `flit-3.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
-requires = ["flit_core >=3.8.0,<4"]
+requires = ["flit_core >=3.9.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "flit"
 authors = [
     {name = "Thomas Kluyver", email = "thomas@kluyver.me.uk"},
 ]
 dependencies = [
-    "flit_core >=3.8.0",
+    "flit_core >=3.9.0",
     "requests",
     "docutils",
     "tomli-w",
 ]
 requires-python = ">=3.6"
 readme = "README.rst"
 license = {file = "LICENSE"}
```

### Comparing `flit-3.8.0/tests/test_build.py` & `flit-3.9.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_find_python_executable.py` & `flit-3.9.0/tests/test_find_python_executable.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_init.py` & `flit-3.9.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_install.py` & `flit-3.9.0/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_sdist.py` & `flit-3.9.0/tests/test_sdist.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_tomlify.py` & `flit-3.9.0/tests/test_tomlify.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_upload.py` & `flit-3.9.0/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_validate.py` & `flit-3.9.0/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_vcs.py` & `flit-3.9.0/tests/test_vcs.py`

 * *Files identical despite different names*

### Comparing `flit-3.8.0/tests/test_wheel.py` & `flit-3.9.0/tests/test_wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import configparser
 import os
+import stat
 from pathlib import Path
 import tempfile
 from unittest import skipIf
 import zipfile
 
 import pytest
 from testpath import assert_isfile, assert_isdir, assert_not_path_exists
@@ -195,14 +196,18 @@
         perms = (info.external_attr >> 16) & 0o777
         assert perms == 0o755, oct(perms)
 
         info = zf.getinfo('module1-0.1.dist-info/METADATA')
         perms = (info.external_attr >> 16) & 0o777
         assert perms == 0o644, oct(perms)
 
+        info = zf.getinfo('module1-0.1.dist-info/RECORD')
+        perms = (info.external_attr >> 16) & stat.S_IFREG
+        assert perms
+
 def test_compression(tmp_path):
     info = make_wheel_in(samples_dir / 'module1_toml' / 'pyproject.toml', tmp_path)
     assert_isfile(info.file)
     with zipfile.ZipFile(str(info.file)) as zf:
         for name in [
             'module1.py',
             'module1-0.1.dist-info/METADATA',
```

### Comparing `flit-3.8.0/tox.ini` & `flit-3.9.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 commands =
     python -m pytest --cov=flit --cov=flit_core/flit_core
 
 [testenv:bootstrap]
 skip_install = true
 # Make the install step a no-op, so nothing gets installed in the env
 install_command = true {packages}
-whitelist_externals = true
+allowlist_externals = true
 changedir = flit_core
 commands =
     python -c "from flit_core.buildapi import build_wheel;\
                from tempfile import mkdtemp;\
                build_wheel(mkdtemp())"
```

### Comparing `flit-3.8.0/PKG-INFO` & `flit-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: flit
-Version: 3.8.0
+Version: 3.9.0
 Summary: A simple packaging tool for simple packages.
 Author-email: Thomas Kluyver <thomas@kluyver.me.uk>
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: flit_core >=3.8.0
+Requires-Dist: flit_core >=3.9.0
 Requires-Dist: requests
 Requires-Dist: docutils
 Requires-Dist: tomli-w
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinxcontrib_github_alt ; extra == "doc"
 Requires-Dist: pygments-github-lexers ; extra == "doc"
 Requires-Dist: testpath ; extra == "test"
```

