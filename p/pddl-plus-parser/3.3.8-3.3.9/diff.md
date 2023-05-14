# Comparing `tmp/pddl-plus-parser-3.3.8.tar.gz` & `tmp/pddl-plus-parser-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pddl-plus-parser-3.3.8.tar", last modified: Sun Apr 30 16:46:50 2023, max compression
+gzip compressed data, was "pddl-plus-parser-3.3.9.tar", last modified: Mon May  1 08:11:48 2023, max compression
```

## Comparing `pddl-plus-parser-3.3.8.tar` & `pddl-plus-parser-3.3.9.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:50.018113 pddl-plus-parser-3.3.8/
--rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.3.8/LICENSE
--rw-rw-rw-   0        0        0     1519 2023-04-30 16:46:50.018113 pddl-plus-parser-3.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1249 2023-04-17 12:20:18.000000 pddl-plus-parser-3.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.950536 pddl-plus-parser-3.3.8/pddl_plus_parser/
--rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.959536 pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/
--rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/__init__.py
--rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/domain_exporter.py
--rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/enhsp_output_parser.py
--rw-rw-rw-   0        0        0     3613 2022-06-02 06:33:08.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/ff_output_parser.py
--rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
--rw-rw-rw-   0        0        0     4458 2022-08-21 11:50:38.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/problem_exporter.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.967524 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/
--rw-rw-rw-   0        0        0      376 2023-04-17 14:54:54.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/__init__.py
--rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/domain_parser.py
--rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/effects_parser.py
--rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/parsing_utils.py
--rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
--rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
--rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/preconditions_parser.py
--rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/problem_parser.py
--rw-rw-rw-   0        0        0    10281 2023-02-20 11:23:13.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/trajectory_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.983523 pddl-plus-parser-3.3.8/pddl_plus_parser/models/
--rw-rw-rw-   0        0        0      929 2023-04-09 14:33:10.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/__init__.py
--rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/action_call.py
--rw-rw-rw-   0        0        0     1853 2023-04-13 11:59:48.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/conditional_effect.py
--rw-rw-rw-   0        0        0     5945 2023-04-17 10:57:12.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/grounded_effect.py
--rw-rw-rw-   0        0        0    13069 2023-04-30 16:17:41.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/grounded_precondition.py
--rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/grounding_utils.py
--rw-rw-rw-   0        0        0     7500 2023-04-16 13:28:59.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/numerical_expression.py
--rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/observation.py
--rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_action.py
--rw-rw-rw-   0        0        0     1415 2022-08-21 09:16:42.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_domain.py
--rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_function.py
--rw-rw-rw-   0        0        0      372 2022-01-17 15:22:52.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_object.py
--rw-rw-rw-   0        0        0     8653 2023-04-30 16:08:01.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_operator.py
--rw-rw-rw-   0        0        0     9709 2023-04-27 10:37:17.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_precondition.py
--rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_predicate.py
--rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_problem.py
--rw-rw-rw-   0        0        0     2845 2023-04-30 16:46:24.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_state.py
--rw-rw-rw-   0        0        0     1135 2022-03-15 08:50:58.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_type.py
--rw-rw-rw-   0        0        0     1865 2023-04-09 08:35:12.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/models/universal_quantifier.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.989536 pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/
--rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/common.py
--rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
--rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
--rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
--rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.997542 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/
--rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/__init__.py
--rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/common.py
--rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/counters_generator.py
--rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/depots_generator.py
--rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/farmland_generator.py
--rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/plant_watering_generator.py
--rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/sailing_generator.py
--rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/settlers_problem_generator.py
--rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/zenotravel_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.954536 pddl-plus-parser-3.3.8/pddl_plus_parser.egg-info/
--rw-rw-rw-   0        0        0     1519 2023-04-30 16:46:49.000000 pddl-plus-parser-3.3.8/pddl_plus_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3567 2023-04-30 16:46:49.000000 pddl-plus-parser-3.3.8/pddl_plus_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 16:46:49.000000 pddl-plus-parser-3.3.8/pddl_plus_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-30 16:46:49.000000 pddl-plus-parser-3.3.8/pddl_plus_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 16:46:50.019126 pddl-plus-parser-3.3.8/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-04-30 16:46:47.000000 pddl-plus-parser-3.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.947536 pddl-plus-parser-3.3.8/tests/
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:49.999530 pddl-plus-parser-3.3.8/tests/exporters_tests/
--rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.3.8/tests/exporters_tests/__init__.py
--rw-rw-rw-   0        0        0    10765 2023-04-30 16:18:40.000000 pddl-plus-parser-3.3.8/tests/exporters_tests/numeric_trajectory_exporter_test.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:50.004561 pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/
--rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/__init__.py
--rw-rw-rw-   0        0        0     3288 2023-04-17 12:07:14.000000 pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/consts.py
--rw-rw-rw-   0        0        0    39905 2023-04-17 12:16:07.000000 pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/domain_parser_test.py
--rw-rw-rw-   0        0        0     3578 2023-04-09 11:50:45.000000 pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/pddl_tokenizer_test.py
--rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/problem_parser_test.py
--rw-rw-rw-   0        0        0     6285 2023-02-21 16:00:23.000000 pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/trajectory_parser_test.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:50.011561 pddl-plus-parser-3.3.8/tests/models_tests/
--rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.3.8/tests/models_tests/__init__.py
--rw-rw-rw-   0        0        0      427 2022-12-05 14:12:59.000000 pddl-plus-parser-3.3.8/tests/models_tests/consts.py
--rw-rw-rw-   0        0        0    15208 2023-04-17 10:08:25.000000 pddl-plus-parser-3.3.8/tests/models_tests/grounded_effect_test.py
--rw-rw-rw-   0        0        0    25195 2023-04-30 16:17:00.000000 pddl-plus-parser-3.3.8/tests/models_tests/grounded_precondition_test.py
--rw-rw-rw-   0        0        0     3516 2022-06-08 11:36:39.000000 pddl-plus-parser-3.3.8/tests/models_tests/numerical_expression_test.py
--rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.3.8/tests/models_tests/operator_test.py
--rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.3.8/tests/models_tests/pddl_function_test.py
--rw-rw-rw-   0        0        0     6075 2023-04-27 10:33:43.000000 pddl-plus-parser-3.3.8/tests/models_tests/pddl_precondition_test.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:46:50.017113 pddl-plus-parser-3.3.8/tests/multi_agent_tests/
--rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.3.8/tests/multi_agent_tests/__init__.py
--rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.3.8/tests/multi_agent_tests/consts.py
--rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.3.8/tests/multi_agent_tests/multi_agent_domain_converter_test.py
--rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.3.8/tests/multi_agent_tests/multi_agent_problem_converter_test.py
--rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.3.8/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
--rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.3.8/tests/multi_agent_tests/single_agent_plan_converter_test.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.074838 pddl-plus-parser-3.3.9/
+-rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.3.9/LICENSE
+-rw-rw-rw-   0        0        0     1519 2023-05-01 08:11:48.074838 pddl-plus-parser-3.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1249 2023-04-17 12:20:18.000000 pddl-plus-parser-3.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.957041 pddl-plus-parser-3.3.9/pddl_plus_parser/
+-rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.971779 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/
+-rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/__init__.py
+-rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/domain_exporter.py
+-rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/enhsp_output_parser.py
+-rw-rw-rw-   0        0        0     3613 2022-06-02 06:33:08.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/ff_output_parser.py
+-rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
+-rw-rw-rw-   0        0        0     4458 2022-08-21 11:50:38.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/problem_exporter.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.985771 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/
+-rw-rw-rw-   0        0        0      376 2023-04-17 14:54:54.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/__init__.py
+-rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/domain_parser.py
+-rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/effects_parser.py
+-rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/parsing_utils.py
+-rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
+-rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
+-rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/preconditions_parser.py
+-rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/problem_parser.py
+-rw-rw-rw-   0        0        0    10281 2023-02-20 11:23:13.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/trajectory_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.013235 pddl-plus-parser-3.3.9/pddl_plus_parser/models/
+-rw-rw-rw-   0        0        0      835 2023-05-01 08:05:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/__init__.py
+-rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/action_call.py
+-rw-rw-rw-   0        0        0     1935 2023-05-01 08:11:11.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/conditional_effect.py
+-rw-rw-rw-   0        0        0     5945 2023-04-17 10:57:12.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounded_effect.py
+-rw-rw-rw-   0        0        0    13069 2023-04-30 16:17:41.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounded_precondition.py
+-rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounding_utils.py
+-rw-rw-rw-   0        0        0     7500 2023-04-16 13:28:59.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/numerical_expression.py
+-rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/observation.py
+-rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_action.py
+-rw-rw-rw-   0        0        0     1415 2022-08-21 09:16:42.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_domain.py
+-rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_function.py
+-rw-rw-rw-   0        0        0      372 2022-01-17 15:22:52.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_object.py
+-rw-rw-rw-   0        0        0     8653 2023-04-30 16:08:01.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_operator.py
+-rw-rw-rw-   0        0        0     9709 2023-04-27 10:37:17.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_precondition.py
+-rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_predicate.py
+-rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_problem.py
+-rw-rw-rw-   0        0        0     2845 2023-04-30 16:46:24.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_state.py
+-rw-rw-rw-   0        0        0     1135 2022-03-15 08:50:58.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_type.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.022755 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/
+-rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/common.py
+-rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
+-rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
+-rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
+-rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.037780 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/
+-rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/__init__.py
+-rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/common.py
+-rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/counters_generator.py
+-rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/depots_generator.py
+-rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/farmland_generator.py
+-rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/plant_watering_generator.py
+-rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/sailing_generator.py
+-rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/settlers_problem_generator.py
+-rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/zenotravel_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.963040 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/
+-rw-rw-rw-   0        0        0     1519 2023-05-01 08:11:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3519 2023-05-01 08:11:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 08:11:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:11:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 08:11:48.075839 pddl-plus-parser-3.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-05-01 08:11:35.000000 pddl-plus-parser-3.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.953025 pddl-plus-parser-3.3.9/tests/
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.040780 pddl-plus-parser-3.3.9/tests/exporters_tests/
+-rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.3.9/tests/exporters_tests/__init__.py
+-rw-rw-rw-   0        0        0    10765 2023-04-30 16:18:40.000000 pddl-plus-parser-3.3.9/tests/exporters_tests/numeric_trajectory_exporter_test.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.050301 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/__init__.py
+-rw-rw-rw-   0        0        0     3288 2023-04-17 12:07:14.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/consts.py
+-rw-rw-rw-   0        0        0    39905 2023-04-17 12:16:07.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/domain_parser_test.py
+-rw-rw-rw-   0        0        0     3578 2023-04-09 11:50:45.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/pddl_tokenizer_test.py
+-rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/problem_parser_test.py
+-rw-rw-rw-   0        0        0     6285 2023-02-21 16:00:23.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/trajectory_parser_test.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.062837 pddl-plus-parser-3.3.9/tests/models_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.3.9/tests/models_tests/__init__.py
+-rw-rw-rw-   0        0        0      427 2022-12-05 14:12:59.000000 pddl-plus-parser-3.3.9/tests/models_tests/consts.py
+-rw-rw-rw-   0        0        0    15208 2023-04-17 10:08:25.000000 pddl-plus-parser-3.3.9/tests/models_tests/grounded_effect_test.py
+-rw-rw-rw-   0        0        0    25195 2023-04-30 16:17:00.000000 pddl-plus-parser-3.3.9/tests/models_tests/grounded_precondition_test.py
+-rw-rw-rw-   0        0        0     3516 2022-06-08 11:36:39.000000 pddl-plus-parser-3.3.9/tests/models_tests/numerical_expression_test.py
+-rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.3.9/tests/models_tests/operator_test.py
+-rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.3.9/tests/models_tests/pddl_function_test.py
+-rw-rw-rw-   0        0        0     6075 2023-04-27 10:33:43.000000 pddl-plus-parser-3.3.9/tests/models_tests/pddl_precondition_test.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.072839 pddl-plus-parser-3.3.9/tests/multi_agent_tests/
+-rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/__init__.py
+-rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/consts.py
+-rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_domain_converter_test.py
+-rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_problem_converter_test.py
+-rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
+-rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/single_agent_plan_converter_test.py
```

### Comparing `pddl-plus-parser-3.3.8/LICENSE` & `pddl-plus-parser-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/PKG-INFO` & `pddl-plus-parser-3.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.3.8
+Version: 3.3.9
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDDL Plus Parser
```

### Comparing `pddl-plus-parser-3.3.8/README.md` & `pddl-plus-parser-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/domain_exporter.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/domain_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/enhsp_output_parser.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/enhsp_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/ff_output_parser.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/ff_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/numeric_trajectory_exporter.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/numeric_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/exporters/problem_exporter.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/problem_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/domain_parser.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/domain_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/effects_parser.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/effects_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/parsing_utils.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/preconditions_parser.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/preconditions_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/problem_parser.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/problem_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/lisp_parsers/trajectory_parser.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/trajectory_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/__init__.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 from .pddl_object import PDDLObject, PDDLConstant
 from .pddl_operator import Operator, NOPOperator
 from .pddl_precondition import Precondition, CompoundPrecondition, UniversalPrecondition
 from .pddl_predicate import SignatureType, Predicate, GroundedPredicate
 from .pddl_problem import Problem
 from .pddl_state import State
 from .pddl_type import PDDLType
-from .universal_quantifier import UniversalQuantifiedPrecondition, UniversalQuantifiedEffect
```

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/action_call.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/action_call.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/conditional_effect.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/conditional_effect.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,10 +39,12 @@
         self.quantified_type = quantified_type
         self.conditional_effects = set()
 
     def __str__(self):
         if len(self.conditional_effects) == 0:
             return ""
 
-        conditional_effects = "\n\t".join([str(conditional_effect) for conditional_effect in self.conditional_effects])
-        return f"(forall ({self.quantified_parameter} - {self.quantified_type.name})" \
-               f"\n\t\t{conditional_effects})"
+        combined_universal_effect = ""
+        for conditional_effect in self.conditional_effects:
+            combined_universal_effect += f"(forall ({self.quantified_parameter} - {self.quantified_type.name})" \
+                                         f"\n\t\t{str(conditional_effect)})\n\t"
+        return combined_universal_effect
```

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/grounded_effect.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounded_effect.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/grounded_precondition.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounded_precondition.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/grounding_utils.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounding_utils.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/numerical_expression.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/numerical_expression.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/observation.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/observation.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_action.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_action.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_domain.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_domain.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_function.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_function.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_operator.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_operator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_precondition.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_precondition.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_predicate.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_predicate.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_problem.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_problem.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_state.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_state.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/models/pddl_type.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_type.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/common.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/common.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/multi_agent/single_agent_plan_converter.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/single_agent_plan_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/counters_generator.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/counters_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/depots_generator.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/depots_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/farmland_generator.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/farmland_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/plant_watering_generator.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/plant_watering_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/sailing_generator.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/sailing_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/settlers_problem_generator.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/settlers_problem_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser/problem_generators/zenotravel_generator.py` & `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/zenotravel_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser.egg-info/PKG-INFO` & `pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.3.8
+Version: 3.3.9
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDDL Plus Parser
```

### Comparing `pddl-plus-parser-3.3.8/pddl_plus_parser.egg-info/SOURCES.txt` & `pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 pddl_plus_parser/models/pddl_object.py
 pddl_plus_parser/models/pddl_operator.py
 pddl_plus_parser/models/pddl_precondition.py
 pddl_plus_parser/models/pddl_predicate.py
 pddl_plus_parser/models/pddl_problem.py
 pddl_plus_parser/models/pddl_state.py
 pddl_plus_parser/models/pddl_type.py
-pddl_plus_parser/models/universal_quantifier.py
 pddl_plus_parser/multi_agent/__init__.py
 pddl_plus_parser/multi_agent/common.py
 pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
 pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
 pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
 pddl_plus_parser/multi_agent/single_agent_plan_converter.py
 pddl_plus_parser/problem_generators/__init__.py
```

### Comparing `pddl-plus-parser-3.3.8/tests/exporters_tests/numeric_trajectory_exporter_test.py` & `pddl-plus-parser-3.3.9/tests/exporters_tests/numeric_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/consts.py` & `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/domain_parser_test.py` & `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/domain_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/pddl_tokenizer_test.py` & `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/pddl_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/problem_parser_test.py` & `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/problem_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/lisp_parsers_tests/trajectory_parser_test.py` & `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/trajectory_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/models_tests/grounded_effect_test.py` & `pddl-plus-parser-3.3.9/tests/models_tests/grounded_effect_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/models_tests/grounded_precondition_test.py` & `pddl-plus-parser-3.3.9/tests/models_tests/grounded_precondition_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/models_tests/numerical_expression_test.py` & `pddl-plus-parser-3.3.9/tests/models_tests/numerical_expression_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/models_tests/operator_test.py` & `pddl-plus-parser-3.3.9/tests/models_tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/models_tests/pddl_function_test.py` & `pddl-plus-parser-3.3.9/tests/models_tests/pddl_function_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/models_tests/pddl_precondition_test.py` & `pddl-plus-parser-3.3.9/tests/models_tests/pddl_precondition_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/multi_agent_tests/consts.py` & `pddl-plus-parser-3.3.9/tests/multi_agent_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/multi_agent_tests/multi_agent_domain_converter_test.py` & `pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_domain_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/multi_agent_tests/multi_agent_problem_converter_test.py` & `pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_problem_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py` & `pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.8/tests/multi_agent_tests/single_agent_plan_converter_test.py` & `pddl-plus-parser-3.3.9/tests/multi_agent_tests/single_agent_plan_converter_test.py`

 * *Files identical despite different names*

