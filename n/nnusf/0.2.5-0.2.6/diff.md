# Comparing `tmp/nnusf-0.2.5.tar.gz` & `tmp/nnusf-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnusf-0.2.5.tar", max compression
+gzip compressed data, was "nnusf-0.2.6.tar", max compression
```

## Comparing `nnusf-0.2.5.tar` & `nnusf-0.2.6.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0    35149 2023-04-11 21:01:32.595940 nnusf-0.2.5/LICENSE
--rw-r--r--   0        0        0     2606 2023-04-11 21:01:32.595940 nnusf-0.2.5/README.md
--rw-r--r--   0        0        0     2282 2023-04-11 21:03:21.526487 nnusf-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-11 21:03:21.530488 nnusf-0.2.5/src/nnusf/__init__.py
--rw-r--r--   0        0        0      133 2023-04-11 21:01:32.719948 nnusf-0.2.5/src/nnusf/cli/__init__.py
--rw-r--r--   0        0        0      172 2023-04-11 21:01:32.719948 nnusf-0.2.5/src/nnusf/cli/base.py
--rw-r--r--   0        0        0     4109 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/data.py
--rw-r--r--   0        0        0     2082 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/extra.py
--rw-r--r--   0        0        0     3407 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/fit.py
--rw-r--r--   0        0        0      201 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/log.py
--rw-r--r--   0        0        0     5284 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/plot.py
--rw-r--r--   0        0        0      879 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/report.py
--rw-r--r--   0        0        0     6815 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/theory.py
--rw-r--r--   0        0        0      277 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/__init__.py
--rw-r--r--   0        0        0     2989 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/coefficients.py
--rw-r--r--   0        0        0     1002 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/combine_tables.py
--rw-r--r--   0        0        0     1439 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/filters.py
--rw-r--r--   0        0        0     6470 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/loader.py
--rw-r--r--   0        0        0     9416 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/matching_grids.py
--rw-r--r--   0        0        0    13188 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/utils.py
--rwxr-xr-x   0        0        0     6128 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_bebcwa59.py
--rwxr-xr-x   0        0        0     6675 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_ccfr.py
--rwxr-xr-x   0        0        0    17661 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_cdhsw.py
--rwxr-xr-x   0        0        0    10365 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_charm.py
--rwxr-xr-x   0        0        0    11707 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_chorus.py
--rwxr-xr-x   0        0        0     9449 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_nutev.py
--rw-r--r--   0        0        0      104 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/get/__init__.py
--rw-r--r--   0        0        0      172 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/get/base.py
--rw-r--r--   0        0        0      698 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/get/gettheory.py
--rw-r--r--   0        0        0      201 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/get/log.py
--rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/lhapdf/__init__.py
--rw-r--r--   0        0        0     6001 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/lhapdf/dump_grids.py
--rw-r--r--   0        0        0     9503 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/lhapdf/utils.py
--rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/__init__.py
--rw-r--r--   0        0        0     7303 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/covmat.py
--rw-r--r--   0        0        0    17946 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/fit.py
--rw-r--r--   0        0        0     4344 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/kinematics.py
--rw-r--r--   0        0        0     3559 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/matching.py
--rw-r--r--   0        0        0     2952 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/sf.py
--rw-r--r--   0        0        0     6132 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/th_covmat.py
--rw-r--r--   0        0        0     7191 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/utils.py
--rw-r--r--   0        0        0     1384 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plotstyle.mplstyle
--rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/__init__.py
--rw-r--r--   0        0        0     7125 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/assets/index.html
--rwxr-xr-x   0        0        0    68365 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/assets/report.css
--rw-r--r--   0        0        0     9969 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/genfiles.py
--rw-r--r--   0        0        0     5641 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/genhtml.py
--rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/scripts/__init__.py
--rw-r--r--   0        0        0     2370 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/scripts/gettheory.py
--rw-r--r--   0        0        0     1369 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/scripts/integrate.py
--rw-r--r--   0        0        0     3315 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/scripts/isoscalar.py
--rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/__init__.py
--rw-r--r--   0        0        0     5283 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/callbacks.py
--rw-r--r--   0        0        0     3339 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/compute_expchi2.py
--rw-r--r--   0        0        0     2957 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/layers.py
--rw-r--r--   0        0        0     3926 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/load_data.py
--rw-r--r--   0        0        0     4238 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/load_fit_data.py
--rw-r--r--   0        0        0     5351 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/model_gen.py
--rw-r--r--   0        0        0     2603 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/postfit.py
--rw-r--r--   0        0        0     3120 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/run_sffit.py
--rw-r--r--   0        0        0     2241 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/scaling.py
--rw-r--r--   0        0        0    11423 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/sum_rules.py
--rw-r--r--   0        0        0     2728 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/train_model.py
--rw-r--r--   0        0        0     8001 2023-04-11 21:01:32.727949 nnusf-0.2.5/src/nnusf/sffit/utils.py
--rw-r--r--   0        0        0        0 2023-04-11 21:01:32.727949 nnusf-0.2.5/src/nnusf/theory/__init__.py
--rw-r--r--   0        0        0  1626320 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/assets/genie.hdf5
--rw-r--r--   0        0        0      649 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/assets/theory_nnusf.yaml
--rw-r--r--   0        0        0     1245 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/bodek_yang/__init__.py
--rw-r--r--   0        0        0      157 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/bodek_yang/cuts.py
--rw-r--r--   0        0        0     1532 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/bodek_yang/load.py
--rw-r--r--   0        0        0      800 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/bodek_yang/runcards.py
--rw-r--r--   0        0        0     4209 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/compare_to_data.py
--rw-r--r--   0        0        0       47 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/data_vs_theory/__init__.py
--rw-r--r--   0        0        0      646 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/data_vs_theory/runcards.py
--rw-r--r--   0        0        0      885 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/defs.py
--rw-r--r--   0        0        0     1991 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/grids.py
--rw-r--r--   0        0        0       47 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/highq/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/highq/load.py
--rw-r--r--   0        0        0     3960 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/highq/runcards.py
--rw-r--r--   0        0        0    12073 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/predictions.py
--rw-r--r--   0        0        0     5969 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/runcards.py
--rw-r--r--   0        0        0       47 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/yadknots/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/yadknots/runcards.py
--rw-r--r--   0        0        0     6366 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/utils.py
--rw-r--r--   0        0        0     1610 2023-04-11 21:01:32.739949 nnusf-0.2.5/tests/test_loader.py
--rw-r--r--   0        0        0      156 2023-04-11 21:01:32.739949 nnusf-0.2.5/tests/theory/test_bodek_yang.py
--rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 nnusf-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-14 09:19:38.702520 nnusf-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2606 2023-05-14 09:19:38.702520 nnusf-0.2.6/README.md
+-rw-r--r--   0        0        0     2281 2023-05-14 09:21:33.418794 nnusf-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-05-14 09:21:33.422794 nnusf-0.2.6/src/nnusf/__init__.py
+-rw-r--r--   0        0        0      133 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/__init__.py
+-rw-r--r--   0        0        0      172 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/base.py
+-rw-r--r--   0        0        0     4109 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/data.py
+-rw-r--r--   0        0        0     2082 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/extra.py
+-rw-r--r--   0        0        0     3407 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/fit.py
+-rw-r--r--   0        0        0      201 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/log.py
+-rw-r--r--   0        0        0     5735 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/cli/plot.py
+-rw-r--r--   0        0        0      879 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/cli/report.py
+-rw-r--r--   0        0        0     6815 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/cli/theory.py
+-rw-r--r--   0        0        0      277 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/__init__.py
+-rw-r--r--   0        0        0     2989 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/coefficients.py
+-rw-r--r--   0        0        0     1002 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/combine_tables.py
+-rw-r--r--   0        0        0     1439 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/filters.py
+-rw-r--r--   0        0        0     6470 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/loader.py
+-rw-r--r--   0        0        0     9416 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/matching_grids.py
+-rw-r--r--   0        0        0    13188 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/utils.py
+-rwxr-xr-x   0        0        0     6128 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_bebcwa59.py
+-rwxr-xr-x   0        0        0     6675 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_ccfr.py
+-rwxr-xr-x   0        0        0    17661 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_cdhsw.py
+-rwxr-xr-x   0        0        0    10365 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_charm.py
+-rwxr-xr-x   0        0        0    11707 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_chorus.py
+-rwxr-xr-x   0        0        0     9449 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_nutev.py
+-rw-r--r--   0        0        0      104 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/get/__init__.py
+-rw-r--r--   0        0        0      172 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/get/base.py
+-rw-r--r--   0        0        0      698 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/get/gettheory.py
+-rw-r--r--   0        0        0      201 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/get/log.py
+-rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/lhapdf/__init__.py
+-rw-r--r--   0        0        0     6001 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/lhapdf/dump_grids.py
+-rw-r--r--   0        0        0     9503 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/lhapdf/utils.py
+-rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/__init__.py
+-rw-r--r--   0        0        0     7303 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/covmat.py
+-rw-r--r--   0        0        0    17946 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/fit.py
+-rw-r--r--   0        0        0     4344 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/kinematics.py
+-rw-r--r--   0        0        0     3559 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/matching.py
+-rw-r--r--   0        0        0     2952 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/sf.py
+-rw-r--r--   0        0        0     5572 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/sfs_lhapdf.py
+-rw-r--r--   0        0        0     6132 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/th_covmat.py
+-rw-r--r--   0        0        0     7191 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/utils.py
+-rw-r--r--   0        0        0     1384 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plotstyle.mplstyle
+-rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/__init__.py
+-rw-r--r--   0        0        0     7125 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/assets/index.html
+-rwxr-xr-x   0        0        0    68365 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/assets/report.css
+-rw-r--r--   0        0        0     9969 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/genfiles.py
+-rw-r--r--   0        0        0     5641 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/genhtml.py
+-rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/scripts/__init__.py
+-rw-r--r--   0        0        0     2329 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/scripts/gettheory.py
+-rw-r--r--   0        0        0     1369 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/scripts/integrate.py
+-rw-r--r--   0        0        0     3315 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/scripts/isoscalar.py
+-rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/__init__.py
+-rw-r--r--   0        0        0     5283 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/callbacks.py
+-rw-r--r--   0        0        0     3339 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/compute_expchi2.py
+-rw-r--r--   0        0        0     2957 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/layers.py
+-rw-r--r--   0        0        0     3926 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/load_data.py
+-rw-r--r--   0        0        0     4238 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/load_fit_data.py
+-rw-r--r--   0        0        0     5351 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/model_gen.py
+-rw-r--r--   0        0        0     2603 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/postfit.py
+-rw-r--r--   0        0        0     3120 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/run_sffit.py
+-rw-r--r--   0        0        0     2241 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/scaling.py
+-rw-r--r--   0        0        0    11423 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/sum_rules.py
+-rw-r--r--   0        0        0     2728 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/train_model.py
+-rw-r--r--   0        0        0     8001 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/utils.py
+-rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/theory/__init__.py
+-rw-r--r--   0        0        0  1626320 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/assets/genie.hdf5
+-rw-r--r--   0        0        0      649 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/assets/theory_nnusf.yaml
+-rw-r--r--   0        0        0     1245 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/bodek_yang/__init__.py
+-rw-r--r--   0        0        0      157 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/bodek_yang/cuts.py
+-rw-r--r--   0        0        0     1532 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/bodek_yang/load.py
+-rw-r--r--   0        0        0      800 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/bodek_yang/runcards.py
+-rw-r--r--   0        0        0     4209 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/compare_to_data.py
+-rw-r--r--   0        0        0       47 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/data_vs_theory/__init__.py
+-rw-r--r--   0        0        0      646 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/data_vs_theory/runcards.py
+-rw-r--r--   0        0        0      885 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/defs.py
+-rw-r--r--   0        0        0     1991 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/grids.py
+-rw-r--r--   0        0        0       47 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/highq/__init__.py
+-rw-r--r--   0        0        0     1377 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/highq/load.py
+-rw-r--r--   0        0        0     3960 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/highq/runcards.py
+-rw-r--r--   0        0        0    12073 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/predictions.py
+-rw-r--r--   0        0        0     5969 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/runcards.py
+-rw-r--r--   0        0        0       47 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/yadknots/__init__.py
+-rw-r--r--   0        0        0     1187 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/yadknots/runcards.py
+-rw-r--r--   0        0        0     6366 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/utils.py
+-rw-r--r--   0        0        0     1610 2023-05-14 09:19:38.822521 nnusf-0.2.6/tests/test_loader.py
+-rw-r--r--   0        0        0      156 2023-05-14 09:19:38.822521 nnusf-0.2.6/tests/theory/test_bodek_yang.py
+-rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 nnusf-0.2.6/PKG-INFO
```

### Comparing `nnusf-0.2.5/LICENSE` & `nnusf-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/README.md` & `nnusf-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/pyproject.toml` & `nnusf-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nnusf"
-version = "0.2.5"
+version = "0.2.6"
 description = "Predictions for all-energy neutrino structure functions"
 readme = "README.md"
 authors = [
   "Alessandro Candido <candido.ale@gmail.com>",
   "Alfonso Garcia <pochoarus@msn.com>",
   "Giacomo Magni <giac.magni@gmail.com>",
   "Tanjona R. Rabemananjara <tanjona.lspc@gmail.com>",
@@ -31,15 +31,15 @@
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 h5py = "^3.7.0"
 PyYAML = "^6.0"
 yadism = "^0.12.3"
 pineappl = "^0.5.0"
 matplotlib = "^3.5.2"
-seaborn = "^0.11.2"
+seaborn = "0.12.2"
 pandas = "^1.4.2"
 rich = "^12.5.1"
 scipy = "^1.8.1"
 tensorflow = "<2.9.10"
 pylint = "^2.14.4"
 appdirs = "^1.4.4"
 banana-hep = "^0.6.6"
```

### Comparing `nnusf-0.2.5/src/nnusf/cli/data.py` & `nnusf-0.2.6/src/nnusf/cli/data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/cli/extra.py` & `nnusf-0.2.6/src/nnusf/cli/extra.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/cli/fit.py` & `nnusf-0.2.6/src/nnusf/cli/fit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/cli/plot.py` & `nnusf-0.2.6/src/nnusf/cli/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
 """Provide plot subcommand."""
 import pathlib
 
 import click
 
-from ..plot import covmat, fit, kinematics, matching, sf, th_covmat
+from ..plot import covmat, fit, kinematics, matching, sf, sfs_lhapdf, th_covmat
 from ..theory import defs
 from . import base
 
 
 @base.command.group("plot")
 def subcommand():
     """Provide plot utilities."""
 
 
 dest = click.option(
     "-d",
     "--destination",
     type=click.Path(path_type=pathlib.Path),
     default=pathlib.Path.cwd().absolute() / "plots",
-    help="Alternative destination path to store the resulting plots (default: $PWD/plots).",
+    help="Alternative path to store results (default: $PWD/plots).",
 )
 
 
 @subcommand.command("kin")
 @click.argument(
     "data", nargs=-1, type=click.Path(exists=True, path_type=pathlib.Path)
 )
@@ -59,16 +58,16 @@
     help="""Stringified dictionary of cuts, e.g. '{"Q2": {"min": 1.65}, "W2": {"min": 3.5}}'.""",
 )
 def sub_kinematic(
     data, destination, grouping, wcut, q2max, xlog, ylog, shading, cuts
 ):
     """Generate kinematics plot.
 
-    The plot will include data from each DATA path provided (multiple values allowed),
-    to include all of them just run:
+    The plot will include data from each DATA path provided
+    (multiple values allowed), to include all of them just run:
 
         nnu plot kin commondata/data/*
 
     """
     if cuts is not None:
         cuts = eval(cuts)
 
@@ -118,23 +117,23 @@
     "--individual_data",
     is_flag=True,
     help="Plot the individual datasets.",
 )
 def sub_covmat(data, destination, inverse, norm, cuts, individual_data):
     """Generate covariance matrix heatmap.
 
-    The operation is repeated for each DATA path provided (multiple values allowed),
-    e.g.:
+    The operation is repeated for each DATA path provided
+    (multiple values allowed), e.g.:
 
         nnu plot covmat commondata/data/*
 
     to repeat the operation for all datasets stored in `data`.
 
-    A further plot will be generated, including the full covariance matrix for
-    the union of the datasets selected.
+    A further plot will be generated, including the full covariance
+    matrix for the union of the datasets selected.
 
     """
     if cuts is not None:
         cuts = eval(cuts)
 
     covmat.main(
         data,
@@ -147,19 +146,21 @@
 
 
 @subcommand.command("fit")
 @click.argument("model", type=click.Path(exists=True, path_type=pathlib.Path))
 @click.argument("runcard", type=click.Path(exists=True, path_type=pathlib.Path))
 @dest
 def sub_fit(model, runcard, destination):
-    """Plot predictions from the fit and/or compare them to the experimental
-    measurements. The command takes two positional arguments and one optional
-    argument. The command should be run as follows:
+    """Plot predictions from the fit and/or compare them
+    to the experimental measurements. The command takes
+    two positional arguments and one optional argument.
+    The command should be run as follows:
+
+        nnu plot fit <path_fit_folder> <path_plot_yaml> [-d destination_foder]
 
-        nnu plot fit <path_fit_folder> <path_plot_yaml> [destination_foder]
     """
     fit.main(model, runcard, destination)
 
 
 sfkinds = list(defs.sfmap.keys())
 
 
@@ -183,34 +184,52 @@
 @subcommand.command("matching_dataset")
 @click.argument("dataset", type=click.Path(path_type=pathlib.Path, exists=True))
 @dest
 def sub_matching_dataset(dataset, destination):
     """Plots the matching datasets along with the actual data.
 
     eg: nnu plot matching_dataset commondata/data/DATA_NUTEV_F2_MATCHING.csv
+
     """
     matching.main(dataset, destination)
 
 
 @subcommand.command("th_covmat")
 @click.argument(
     "data", nargs=-1, type=click.Path(exists=True, path_type=pathlib.Path)
 )
 @dest
 @inverse
 @norm
 @cuts
-def sub_covmat(data, destination, inverse, norm, cuts):
+def sub_th_covmat(data, destination, inverse, norm, cuts):
     """Generate theory covariance matrix heatmap.
 
-    The operation is repeated for each MATCHING DATA path provided (multiple values allowed),
-    e.g.:
+    The operation is repeated for each MATCHING DATA path provided
+    (multiple values allowed), e.g.:
 
         nnu plot th_covmat commondata/data/*
+
     """
     th_covmat.main(
         data,
         destination,
         inverse=inverse,
         norm=norm,
         cuts=cuts,
     )
+
+
+@subcommand.command("sfs_lhapdf")
+@click.argument("runcard", type=click.Path(exists=True, path_type=pathlib.Path))
+@dest
+def sub_sfs_lhapdf(runcard, destination):
+    """Plot and/or Compare Structure Function predictions
+    given a run card in which a list of the LHAPDF grid(s)
+    is specified.
+
+    To generate the plot, simply type the following command:
+
+        nnu plot fit <path_to_sfs_runcard> [-d destination]
+
+    """
+    sfs_lhapdf.main(runcard, destination)
```

### Comparing `nnusf-0.2.5/src/nnusf/cli/report.py` & `nnusf-0.2.6/src/nnusf/cli/report.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/cli/theory.py` & `nnusf-0.2.6/src/nnusf/cli/theory.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/data/coefficients.py` & `nnusf-0.2.6/src/nnusf/data/coefficients.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/data/combine_tables.py` & `nnusf-0.2.6/src/nnusf/data/combine_tables.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/data/filters.py` & `nnusf-0.2.6/src/nnusf/data/filters.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/data/loader.py` & `nnusf-0.2.6/src/nnusf/data/loader.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/data/matching_grids.py` & `nnusf-0.2.6/src/nnusf/data/matching_grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/data/utils.py` & `nnusf-0.2.6/src/nnusf/data/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/filters/filter_bebcwa59.py` & `nnusf-0.2.6/src/nnusf/filters/filter_bebcwa59.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/filters/filter_ccfr.py` & `nnusf-0.2.6/src/nnusf/filters/filter_ccfr.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/filters/filter_cdhsw.py` & `nnusf-0.2.6/src/nnusf/filters/filter_cdhsw.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/filters/filter_charm.py` & `nnusf-0.2.6/src/nnusf/filters/filter_charm.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/filters/filter_chorus.py` & `nnusf-0.2.6/src/nnusf/filters/filter_chorus.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/filters/filter_nutev.py` & `nnusf-0.2.6/src/nnusf/filters/filter_nutev.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/get/gettheory.py` & `nnusf-0.2.6/src/nnusf/get/gettheory.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/lhapdf/dump_grids.py` & `nnusf-0.2.6/src/nnusf/lhapdf/dump_grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/lhapdf/utils.py` & `nnusf-0.2.6/src/nnusf/lhapdf/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/plot/covmat.py` & `nnusf-0.2.6/src/nnusf/plot/covmat.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/plot/fit.py` & `nnusf-0.2.6/src/nnusf/plot/fit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/plot/kinematics.py` & `nnusf-0.2.6/src/nnusf/plot/kinematics.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/plot/matching.py` & `nnusf-0.2.6/src/nnusf/plot/matching.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/plot/sf.py` & `nnusf-0.2.6/src/nnusf/plot/sf.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/plot/th_covmat.py` & `nnusf-0.2.6/src/nnusf/plot/th_covmat.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/plot/utils.py` & `nnusf-0.2.6/src/nnusf/plot/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/plotstyle.mplstyle` & `nnusf-0.2.6/src/nnusf/plotstyle.mplstyle`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/reports/assets/index.html` & `nnusf-0.2.6/src/nnusf/reports/assets/index.html`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/reports/assets/report.css` & `nnusf-0.2.6/src/nnusf/reports/assets/report.css`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/reports/genfiles.py` & `nnusf-0.2.6/src/nnusf/reports/genfiles.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/reports/genhtml.py` & `nnusf-0.2.6/src/nnusf/reports/genhtml.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/scripts/gettheory.py` & `nnusf-0.2.6/src/nnusf/scripts/gettheory.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import logging
 import requests
 import tarfile
 import tempfile
 
 from appdirs import AppDirs
 from pathlib import Path
-from typing import Optional
 
 _logger = logging.getLogger(__name__)
 
 
 def setup_directory(dirname: str) -> Path:
     """Set up the user data directories.
-    
+
     Parameters:
     -----------
     dirname: str
         Name of the App directory
-    
+
     Returns:
     --------
     pathlib.Path:
         Path to the user data folder
     """
     dirs = AppDirs(dirname, "nnsfnu")
     return Path(dirs.user_data_dir)
@@ -59,22 +58,22 @@
         ofile.write(response.raw.read())
     _logger.info(f"Theory downloaded succesfully in '{tempdir}'")
 
 
 def get_theory(userdir: Path) -> None:
     """Download the theory in a temporary directory and
     extract it to the user data folder.
-    
+
     Parameters:
     -----------
     userdir: Path
         Path to the user data folder
     """
     name = "nnusf_data.tar.gz"
-    url = f"https://data.nnpdf.science/NNSFnu/data/{name}"
+    url = f"https://data.nnpdf.science/NNUSF/data/{name}"
 
     try:
         response = requests.get(url, stream=True)
         response.raise_for_status()
     except requests.exceptions.HTTPError as err:
         _logger.error(err)
```

### Comparing `nnusf-0.2.5/src/nnusf/scripts/integrate.py` & `nnusf-0.2.6/src/nnusf/scripts/integrate.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/scripts/isoscalar.py` & `nnusf-0.2.6/src/nnusf/scripts/isoscalar.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/callbacks.py` & `nnusf-0.2.6/src/nnusf/sffit/callbacks.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/compute_expchi2.py` & `nnusf-0.2.6/src/nnusf/sffit/compute_expchi2.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/layers.py` & `nnusf-0.2.6/src/nnusf/sffit/layers.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/load_data.py` & `nnusf-0.2.6/src/nnusf/sffit/load_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/load_fit_data.py` & `nnusf-0.2.6/src/nnusf/sffit/load_fit_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/model_gen.py` & `nnusf-0.2.6/src/nnusf/sffit/model_gen.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/postfit.py` & `nnusf-0.2.6/src/nnusf/sffit/postfit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/run_sffit.py` & `nnusf-0.2.6/src/nnusf/sffit/run_sffit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/scaling.py` & `nnusf-0.2.6/src/nnusf/sffit/scaling.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/sum_rules.py` & `nnusf-0.2.6/src/nnusf/sffit/sum_rules.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/train_model.py` & `nnusf-0.2.6/src/nnusf/sffit/train_model.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/sffit/utils.py` & `nnusf-0.2.6/src/nnusf/sffit/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/assets/genie.hdf5` & `nnusf-0.2.6/src/nnusf/theory/assets/genie.hdf5`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/assets/theory_nnusf.yaml` & `nnusf-0.2.6/src/nnusf/theory/assets/theory_nnusf.yaml`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/bodek_yang/__init__.py` & `nnusf-0.2.6/src/nnusf/theory/bodek_yang/__init__.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/bodek_yang/load.py` & `nnusf-0.2.6/src/nnusf/theory/bodek_yang/load.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/bodek_yang/runcards.py` & `nnusf-0.2.6/src/nnusf/theory/bodek_yang/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/compare_to_data.py` & `nnusf-0.2.6/src/nnusf/theory/compare_to_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/data_vs_theory/runcards.py` & `nnusf-0.2.6/src/nnusf/theory/data_vs_theory/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/defs.py` & `nnusf-0.2.6/src/nnusf/theory/defs.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/grids.py` & `nnusf-0.2.6/src/nnusf/theory/grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/highq/load.py` & `nnusf-0.2.6/src/nnusf/theory/highq/load.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/highq/runcards.py` & `nnusf-0.2.6/src/nnusf/theory/highq/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/predictions.py` & `nnusf-0.2.6/src/nnusf/theory/predictions.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/runcards.py` & `nnusf-0.2.6/src/nnusf/theory/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/theory/yadknots/runcards.py` & `nnusf-0.2.6/src/nnusf/theory/yadknots/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/src/nnusf/utils.py` & `nnusf-0.2.6/src/nnusf/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/tests/test_loader.py` & `nnusf-0.2.6/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.5/PKG-INFO` & `nnusf-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnusf
-Version: 0.2.5
+Version: 0.2.6
 Summary: Predictions for all-energy neutrino structure functions
 Home-page: https://github.com/NNPDF/nnusf
 Author: Alessandro Candido
 Author-email: candido.ale@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -27,15 +27,15 @@
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pineappl (>=0.5.0,<0.6.0)
 Requires-Dist: pygit2 (>=1.10.1,<2.0.0)
 Requires-Dist: pylint (>=2.14.4,<3.0.0)
 Requires-Dist: pytzdata (>=2020.1,<2021.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
-Requires-Dist: seaborn (>=0.11.2,<0.12.0)
+Requires-Dist: seaborn (==0.12.2)
 Requires-Dist: setuptools (>=65.5.1,<66.0.0)
 Requires-Dist: tensorflow (<2.9.10)
 Requires-Dist: termcolor (==1.1.0)
 Requires-Dist: yadism (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/NNPDF/nnusf
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nnusf Version: 0.2.5 Summary: Predictions for all-
+Metadata-Version: 2.1 Name: nnusf Version: 0.2.6 Summary: Predictions for all-
 energy neutrino structure functions Home-page: https://github.com/NNPDF/nnusf
 Author: Alessandro Candido Author-email: candido.ale@gmail.com Requires-Python:
 >=3.9,<3.11 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering Classifier:
@@ -12,15 +12,15 @@
 click (>=8.1.3,<9.0.0) Requires-Dist: greenlet (>=1.1.2,<2.0.0) Requires-Dist:
 h5py (>=3.7.0,<4.0.0) Requires-Dist: matplotlib (>=3.5.2,<4.0.0) Requires-Dist:
 pandas (>=1.4.2,<2.0.0) Requires-Dist: particle (>=0.21.2,<0.22.0) Requires-
 Dist: pendulum (>=2.1.2,<3.0.0) Requires-Dist: pineappl (>=0.5.0,<0.6.0)
 Requires-Dist: pygit2 (>=1.10.1,<2.0.0) Requires-Dist: pylint (>=2.14.4,<3.0.0)
 Requires-Dist: pytzdata (>=2020.1,<2021.0) Requires-Dist: rich
 (>=12.5.1,<13.0.0) Requires-Dist: scipy (>=1.8.1,<2.0.0) Requires-Dist: seaborn
-(>=0.11.2,<0.12.0) Requires-Dist: setuptools (>=65.5.1,<66.0.0) Requires-Dist:
+(==0.12.2) Requires-Dist: setuptools (>=65.5.1,<66.0.0) Requires-Dist:
 tensorflow (<2.9.10) Requires-Dist: termcolor (==1.1.0) Requires-Dist: yadism
 (>=0.12.3,<0.13.0) Project-URL: Repository, https://github.com/NNPDF/nnusf
 Description-Content-Type: text/markdown
                              ****** NNSFÎ½ ******
                [Zenodo] [arXiv] [Docs] [PyPI] [Status] [License]
 NNSFÎ½ is a python module that provides predictions for neutrino structure
 functions. It relies on YADISM for the large-Q region while the low-Q regime is
```

