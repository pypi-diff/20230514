# Comparing `tmp/pyphetools-0.2.7.tar.gz` & `tmp/pyphetools-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.2.7.tar", last modified: Thu Jan 12 09:32:34 2023, max compression
+gzip compressed data, was "pyphetools-0.2.9.tar", last modified: Tue Jan 17 17:04:36 2023, max compression
```

## Comparing `pyphetools-0.2.7.tar` & `pyphetools-0.2.9.tar`

### file list

```diff
@@ -1,70 +1,75 @@
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.382098 pyphetools-0.2.7/
--rw-r--r--   0 robinp   (904623974) 1088672553     1079 2023-01-08 15:20:15.000000 pyphetools-0.2.7/LICENSE
--rw-r--r--   0 robinp   (904623974) 1088672553        0 2023-01-05 13:57:40.000000 pyphetools-0.2.7/MANIFEST.in
--rw-r--r--   0 robinp   (904623974) 1088672553     3240 2023-01-12 09:32:34.381784 pyphetools-0.2.7/PKG-INFO
--rw-r--r--   0 robinp   (904623974) 1088672553     1182 2023-01-09 08:54:14.000000 pyphetools-0.2.7/README.md
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.271275 pyphetools-0.2.7/pyphetools/
--rw-r--r--   0 robinp   (904623974) 1088672553       11 2023-01-09 09:59:57.000000 pyphetools-0.2.7/pyphetools/__init__.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.332045 pyphetools-0.2.7/pyphetools/creation/
--rw-r--r--   0 robinp   (904623974) 1088672553      737 2023-01-10 13:02:20.000000 pyphetools-0.2.7/pyphetools/creation/__init__.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4481 2023-01-10 17:19:32.000000 pyphetools-0.2.7/pyphetools/creation/age_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4783 2023-01-10 18:55:16.000000 pyphetools-0.2.7/pyphetools/creation/case_encoder.py
--rw-r--r--   0 robinp   (904623974) 1088672553     7210 2023-01-10 17:24:17.000000 pyphetools-0.2.7/pyphetools/creation/cohort_encoder.py
--rw-r--r--   0 robinp   (904623974) 1088672553      507 2022-12-13 18:48:29.000000 pyphetools-0.2.7/pyphetools/creation/column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553      240 2023-01-05 13:57:40.000000 pyphetools-0.2.7/pyphetools/creation/constants.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2226 2023-01-10 17:22:11.000000 pyphetools-0.2.7/pyphetools/creation/custom_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2278 2023-01-08 19:22:08.000000 pyphetools-0.2.7/pyphetools/creation/hp_term.py
--rw-r--r--   0 robinp   (904623974) 1088672553      589 2023-01-06 08:02:51.000000 pyphetools-0.2.7/pyphetools/creation/hpo_cr.py
--rw-r--r--   0 robinp   (904623974) 1088672553     5806 2023-01-06 08:08:38.000000 pyphetools-0.2.7/pyphetools/creation/hpo_exact_cr.py
--rw-r--r--   0 robinp   (904623974) 1088672553     6327 2023-01-05 17:11:47.000000 pyphetools-0.2.7/pyphetools/creation/hpo_parser.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4872 2023-01-10 19:49:38.000000 pyphetools-0.2.7/pyphetools/creation/individual.py
--rw-r--r--   0 robinp   (904623974) 1088672553     5382 2023-01-09 09:50:05.000000 pyphetools-0.2.7/pyphetools/creation/metadata.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1980 2023-01-10 17:22:41.000000 pyphetools-0.2.7/pyphetools/creation/option_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1704 2023-01-05 13:57:40.000000 pyphetools-0.2.7/pyphetools/creation/sex_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4043 2023-01-10 12:19:22.000000 pyphetools-0.2.7/pyphetools/creation/simple_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2614 2023-01-05 13:57:40.000000 pyphetools-0.2.7/pyphetools/creation/thresholded_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4821 2023-01-05 13:57:40.000000 pyphetools-0.2.7/pyphetools/creation/variant.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2232 2023-01-05 13:57:40.000000 pyphetools-0.2.7/pyphetools/creation/variant_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     3208 2023-01-05 13:57:40.000000 pyphetools-0.2.7/pyphetools/creation/variant_validator.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.341650 pyphetools-0.2.7/pyphetools/output/
--rw-r--r--   0 robinp   (904623974) 1088672553      226 2023-01-12 08:31:03.000000 pyphetools-0.2.7/pyphetools/output/__init__.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2911 2023-01-12 09:28:21.000000 pyphetools-0.2.7/pyphetools/output/focus_count_table.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1764 2023-01-12 09:08:39.000000 pyphetools-0.2.7/pyphetools/output/hpo_category.py
--rw-r--r--   0 robinp   (904623974) 1088672553      894 2023-01-11 19:10:33.000000 pyphetools-0.2.7/pyphetools/output/phenopacket_ingestor.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4401 2023-01-12 09:11:51.000000 pyphetools-0.2.7/pyphetools/output/simple_patient.py
--rw-r--r--   0 robinp   (904623974) 1088672553     3221 2023-01-11 19:12:11.000000 pyphetools-0.2.7/pyphetools/output/simple_variant.py
--rw-r--r--   0 robinp   (904623974) 1088672553      433 2023-01-12 09:08:00.000000 pyphetools-0.2.7/pyphetools/output/term_count.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.343632 pyphetools-0.2.7/pyphetools/validation/
--rw-r--r--   0 robinp   (904623974) 1088672553        8 2023-01-09 09:58:48.000000 pyphetools-0.2.7/pyphetools/validation/__init__.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.276863 pyphetools-0.2.7/pyphetools.egg-info/
--rw-r--r--   0 robinp   (904623974) 1088672553     3240 2023-01-12 09:32:34.000000 pyphetools-0.2.7/pyphetools.egg-info/PKG-INFO
--rw-r--r--   0 robinp   (904623974) 1088672553     1782 2023-01-12 09:32:34.000000 pyphetools-0.2.7/pyphetools.egg-info/SOURCES.txt
--rw-r--r--   0 robinp   (904623974) 1088672553        1 2023-01-12 09:32:34.000000 pyphetools-0.2.7/pyphetools.egg-info/dependency_links.txt
--rw-r--r--   0 robinp   (904623974) 1088672553       50 2023-01-12 09:32:34.000000 pyphetools-0.2.7/pyphetools.egg-info/requires.txt
--rw-r--r--   0 robinp   (904623974) 1088672553       36 2023-01-12 09:32:34.000000 pyphetools-0.2.7/pyphetools.egg-info/top_level.txt
--rw-r--r--   0 robinp   (904623974) 1088672553     1295 2023-01-12 09:31:03.000000 pyphetools-0.2.7/pyproject.toml
--rw-r--r--   0 robinp   (904623974) 1088672553       38 2023-01-12 09:32:34.382167 pyphetools-0.2.7/setup.cfg
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.350918 pyphetools-0.2.7/test/
--rw-r--r--   0 robinp   (904623974) 1088672553     3297 2023-01-10 10:04:36.000000 pyphetools-0.2.7/test/test_age_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2976 2023-01-11 14:55:19.000000 pyphetools-0.2.7/test/test_case_encoder.py
--rw-r--r--   0 robinp   (904623974) 1088672553     3417 2023-01-09 10:02:09.000000 pyphetools-0.2.7/test/test_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553      475 2023-01-11 14:55:50.000000 pyphetools-0.2.7/test/test_hp_term.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4988 2023-01-09 10:02:26.000000 pyphetools-0.2.7/test/test_hpo_cr.py
--rw-r--r--   0 robinp   (904623974) 1088672553      439 2023-01-09 10:01:54.000000 pyphetools-0.2.7/test/test_hpo_parser.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4361 2023-01-09 10:02:14.000000 pyphetools-0.2.7/test/test_option_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1884 2023-01-09 10:02:22.000000 pyphetools-0.2.7/test/test_threshold_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1451 2023-01-09 10:02:18.000000 pyphetools-0.2.7/test/test_variant.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.261896 pyphetools-0.2.7/venv/
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-01-12 09:32:34.381201 pyphetools-0.2.7/venv/bin/
--rwxr-xr-x   0 robinp   (904623974) 1088672553      626 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2html.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      746 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2html4.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553     1114 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2html5.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      823 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2latex.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      631 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2man.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      796 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2odt.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553     1758 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      633 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      669 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2s5.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      903 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2xetex.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      634 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rst2xml.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      702 2022-12-06 15:23:54.000000 pyphetools-0.2.7/venv/bin/rstpep2html.py
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.928942 pyphetools-0.2.9/
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     1079 2023-01-08 15:20:15.000000 pyphetools-0.2.9/LICENSE
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-05 13:57:40.000000 pyphetools-0.2.9/MANIFEST.in
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     3240 2023-01-17 17:04:36.928547 pyphetools-0.2.9/PKG-INFO
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     1182 2023-01-09 08:54:14.000000 pyphetools-0.2.9/README.md
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.719883 pyphetools-0.2.9/pyphetools/
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)       11 2023-01-09 09:59:57.000000 pyphetools-0.2.9/pyphetools/__init__.py
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.737935 pyphetools-0.2.9/pyphetools/analyze/
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)       36 2023-01-17 15:38:54.000000 pyphetools-0.2.9/pyphetools/analyze/__init__.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     3140 2023-01-17 15:58:59.000000 pyphetools-0.2.9/pyphetools/analyze/downsampler.py
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.813912 pyphetools-0.2.9/pyphetools/creation/
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      737 2023-01-10 13:02:20.000000 pyphetools-0.2.9/pyphetools/creation/__init__.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     4481 2023-01-10 17:19:32.000000 pyphetools-0.2.9/pyphetools/creation/age_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     4783 2023-01-10 18:55:16.000000 pyphetools-0.2.9/pyphetools/creation/case_encoder.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     7210 2023-01-10 17:24:17.000000 pyphetools-0.2.9/pyphetools/creation/cohort_encoder.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      507 2022-12-13 18:48:29.000000 pyphetools-0.2.9/pyphetools/creation/column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      240 2023-01-05 13:57:40.000000 pyphetools-0.2.9/pyphetools/creation/constants.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     2226 2023-01-10 17:22:11.000000 pyphetools-0.2.9/pyphetools/creation/custom_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     2278 2023-01-08 19:22:08.000000 pyphetools-0.2.9/pyphetools/creation/hp_term.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      589 2023-01-06 08:02:51.000000 pyphetools-0.2.9/pyphetools/creation/hpo_cr.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     5806 2023-01-06 08:08:38.000000 pyphetools-0.2.9/pyphetools/creation/hpo_exact_cr.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     6327 2023-01-05 17:11:47.000000 pyphetools-0.2.9/pyphetools/creation/hpo_parser.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     4872 2023-01-10 19:49:38.000000 pyphetools-0.2.9/pyphetools/creation/individual.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     5382 2023-01-09 09:50:05.000000 pyphetools-0.2.9/pyphetools/creation/metadata.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     1980 2023-01-10 17:22:41.000000 pyphetools-0.2.9/pyphetools/creation/option_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     1704 2023-01-05 13:57:40.000000 pyphetools-0.2.9/pyphetools/creation/sex_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     4043 2023-01-10 12:19:22.000000 pyphetools-0.2.9/pyphetools/creation/simple_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     2614 2023-01-05 13:57:40.000000 pyphetools-0.2.9/pyphetools/creation/thresholded_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     4821 2023-01-05 13:57:40.000000 pyphetools-0.2.9/pyphetools/creation/variant.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     2232 2023-01-05 13:57:40.000000 pyphetools-0.2.9/pyphetools/creation/variant_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     3208 2023-01-05 13:57:40.000000 pyphetools-0.2.9/pyphetools/creation/variant_validator.py
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.844190 pyphetools-0.2.9/pyphetools/output/
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      279 2023-01-13 17:42:13.000000 pyphetools-0.2.9/pyphetools/output/__init__.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     3149 2023-01-13 17:53:06.000000 pyphetools-0.2.9/pyphetools/output/detailed_suppl_table.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     5812 2023-01-13 08:45:02.000000 pyphetools-0.2.9/pyphetools/output/focus_count_table.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     2980 2023-01-13 08:44:05.000000 pyphetools-0.2.9/pyphetools/output/hpo_category.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      894 2023-01-11 19:10:33.000000 pyphetools-0.2.9/pyphetools/output/phenopacket_ingestor.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     4508 2023-01-12 18:07:06.000000 pyphetools-0.2.9/pyphetools/output/simple_patient.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     3221 2023-01-11 19:12:11.000000 pyphetools-0.2.9/pyphetools/output/simple_variant.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      433 2023-01-12 09:08:00.000000 pyphetools-0.2.9/pyphetools/output/term_count.py
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.848663 pyphetools-0.2.9/pyphetools/validation/
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)        8 2023-01-09 09:58:48.000000 pyphetools-0.2.9/pyphetools/validation/__init__.py
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.725715 pyphetools-0.2.9/pyphetools.egg-info/
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     3240 2023-01-17 17:04:36.000000 pyphetools-0.2.9/pyphetools.egg-info/PKG-INFO
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     1915 2023-01-17 17:04:36.000000 pyphetools-0.2.9/pyphetools.egg-info/SOURCES.txt
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)        1 2023-01-17 17:04:36.000000 pyphetools-0.2.9/pyphetools.egg-info/dependency_links.txt
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)       50 2023-01-17 17:04:36.000000 pyphetools-0.2.9/pyphetools.egg-info/requires.txt
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)       42 2023-01-17 17:04:36.000000 pyphetools-0.2.9/pyphetools.egg-info/top_level.txt
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     1295 2023-01-17 15:51:41.000000 pyphetools-0.2.9/pyproject.toml
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)       38 2023-01-17 17:04:36.929011 pyphetools-0.2.9/setup.cfg
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.888511 pyphetools-0.2.9/test/
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     3297 2023-01-10 10:04:36.000000 pyphetools-0.2.9/test/test_age_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     2976 2023-01-11 14:55:19.000000 pyphetools-0.2.9/test/test_case_encoder.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     3417 2023-01-09 10:02:09.000000 pyphetools-0.2.9/test/test_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      445 2023-01-12 19:12:15.000000 pyphetools-0.2.9/test/test_hp_term.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      914 2023-01-13 06:22:44.000000 pyphetools-0.2.9/test/test_hpo_category.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     4988 2023-01-09 10:02:26.000000 pyphetools-0.2.9/test/test_hpo_cr.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)      439 2023-01-09 10:01:54.000000 pyphetools-0.2.9/test/test_hpo_parser.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     4361 2023-01-09 10:02:14.000000 pyphetools-0.2.9/test/test_option_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     1884 2023-01-09 10:02:22.000000 pyphetools-0.2.9/test/test_threshold_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) JAX\Domain Users (1088672553)     1451 2023-01-09 10:02:18.000000 pyphetools-0.2.9/test/test_variant.py
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.698463 pyphetools-0.2.9/venv/
+drwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)        0 2023-01-17 17:04:36.927682 pyphetools-0.2.9/venv/bin/
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      626 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2html.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      746 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2html4.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)     1114 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2html5.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      823 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2latex.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      631 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2man.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      796 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2odt.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)     1758 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      633 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      669 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2s5.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      903 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      634 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rst2xml.py
+-rwxr-xr-x   0 robinp   (904623974) JAX\Domain Users (1088672553)      702 2022-12-06 15:23:54.000000 pyphetools-0.2.9/venv/bin/rstpep2html.py
```

### Comparing `pyphetools-0.2.7/LICENSE` & `pyphetools-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/PKG-INFO` & `pyphetools-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.2.7
+Version: 0.2.9
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.2.7/README.md` & `pyphetools-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/__init__.py` & `pyphetools-0.2.9/pyphetools/creation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.2.9/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/case_encoder.py` & `pyphetools-0.2.9/pyphetools/creation/case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.2.9/pyphetools/creation/cohort_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/custom_column_mapper.py` & `pyphetools-0.2.9/pyphetools/creation/custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/hp_term.py` & `pyphetools-0.2.9/pyphetools/creation/hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/hpo_cr.py` & `pyphetools-0.2.9/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.2.9/pyphetools/creation/hpo_exact_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/hpo_parser.py` & `pyphetools-0.2.9/pyphetools/creation/hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/individual.py` & `pyphetools-0.2.9/pyphetools/creation/individual.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/metadata.py` & `pyphetools-0.2.9/pyphetools/creation/metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.2.9/pyphetools/creation/option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.2.9/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/simple_column_mapper.py` & `pyphetools-0.2.9/pyphetools/creation/simple_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.2.9/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/variant.py` & `pyphetools-0.2.9/pyphetools/creation/variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.2.9/pyphetools/creation/variant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/creation/variant_validator.py` & `pyphetools-0.2.9/pyphetools/creation/variant_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/output/phenopacket_ingestor.py` & `pyphetools-0.2.9/pyphetools/output/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools/output/simple_patient.py` & `pyphetools-0.2.9/pyphetools/output/simple_patient.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,17 @@
     def get_sex(self):
         return self._sex
 
     def get_age(self):
         return self._time_at_last_encounter
 
     def get_observed_hpo_d(self):
+        """
+        returns map with key (string) HP id, value, HpTerm from creation submodule
+        """
         return self._observed
 
     def get_excluded_hpo_d(self):
         return self._excluded
 
     def get_variant_d(self):
         return self._variant_d
```

### Comparing `pyphetools-0.2.7/pyphetools/output/simple_variant.py` & `pyphetools-0.2.9/pyphetools/output/simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.2.9/pyphetools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.2.7
+Version: 0.2.9
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.2.7/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.2.9/pyphetools.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 pyproject.toml
 pyphetools/__init__.py
 pyphetools.egg-info/PKG-INFO
 pyphetools.egg-info/SOURCES.txt
 pyphetools.egg-info/dependency_links.txt
 pyphetools.egg-info/requires.txt
 pyphetools.egg-info/top_level.txt
+pyphetools/analyze/__init__.py
+pyphetools/analyze/downsampler.py
 pyphetools/creation/__init__.py
 pyphetools/creation/age_column_mapper.py
 pyphetools/creation/case_encoder.py
 pyphetools/creation/cohort_encoder.py
 pyphetools/creation/column_mapper.py
 pyphetools/creation/constants.py
 pyphetools/creation/custom_column_mapper.py
@@ -25,25 +27,27 @@
 pyphetools/creation/sex_column_mapper.py
 pyphetools/creation/simple_column_mapper.py
 pyphetools/creation/thresholded_column_mapper.py
 pyphetools/creation/variant.py
 pyphetools/creation/variant_column_mapper.py
 pyphetools/creation/variant_validator.py
 pyphetools/output/__init__.py
+pyphetools/output/detailed_suppl_table.py
 pyphetools/output/focus_count_table.py
 pyphetools/output/hpo_category.py
 pyphetools/output/phenopacket_ingestor.py
 pyphetools/output/simple_patient.py
 pyphetools/output/simple_variant.py
 pyphetools/output/term_count.py
 pyphetools/validation/__init__.py
 test/test_age_column_mapper.py
 test/test_case_encoder.py
 test/test_column_mapper.py
 test/test_hp_term.py
+test/test_hpo_category.py
 test/test_hpo_cr.py
 test/test_hpo_parser.py
 test/test_option_column_mapper.py
 test/test_threshold_column_mapper.py
 test/test_variant.py
 venv/bin/rst2html.py
 venv/bin/rst2html4.py
```

### Comparing `pyphetools-0.2.7/pyproject.toml` & `pyphetools-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["notebooks", "test"]
 
 [project]
 name = "pyphetools"
-version = "0.2.7"
+version = "0.2.9"
 requires-python = ">=3.5"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
```

### Comparing `pyphetools-0.2.7/test/test_age_column_mapper.py` & `pyphetools-0.2.9/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/test/test_case_encoder.py` & `pyphetools-0.2.9/test/test_case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/test/test_column_mapper.py` & `pyphetools-0.2.9/test/test_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/test/test_hpo_cr.py` & `pyphetools-0.2.9/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/test/test_option_column_mapper.py` & `pyphetools-0.2.9/test/test_option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/test/test_threshold_column_mapper.py` & `pyphetools-0.2.9/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/test/test_variant.py` & `pyphetools-0.2.9/test/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2html.py` & `pyphetools-0.2.9/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2html4.py` & `pyphetools-0.2.9/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2html5.py` & `pyphetools-0.2.9/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2latex.py` & `pyphetools-0.2.9/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2man.py` & `pyphetools-0.2.9/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2odt.py` & `pyphetools-0.2.9/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.2.9/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2pseudoxml.py` & `pyphetools-0.2.9/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2s5.py` & `pyphetools-0.2.9/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2xetex.py` & `pyphetools-0.2.9/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rst2xml.py` & `pyphetools-0.2.9/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.2.7/venv/bin/rstpep2html.py` & `pyphetools-0.2.9/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

