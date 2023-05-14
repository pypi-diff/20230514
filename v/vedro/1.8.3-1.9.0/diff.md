# Comparing `tmp/vedro-1.8.3.tar.gz` & `tmp/vedro-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-1.8.3.tar", last modified: Sun Dec  4 08:19:31 2022, max compression
+gzip compressed data, was "vedro-1.9.0.tar", last modified: Sun May 14 18:00:25 2023, max compression
```

## Comparing `vedro-1.8.3.tar` & `vedro-1.9.0.tar`

### file list

```diff
@@ -1,162 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:31.001702 vedro-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-04 08:19:20.000000 vedro-1.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2022-12-04 08:19:31.001702 vedro-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2022-12-04 08:19:20.000000 vedro-1.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-12-04 08:19:31.001702 vedro-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2022-12-04 08:19:20.000000 vedro-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.981701 vedro-1.8.3/vedro/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.985702 vedro-1.8.3/vedro/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.985702 vedro-1.8.3/vedro/core/_config_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_config_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_config_loader/_config_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_config_loader/_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_config_loader/_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_exc_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_lifecycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.985702 vedro-1.8.3/vedro/core/_module_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_module_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_module_loader/_module_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_module_loader/_module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.985702 vedro-1.8.3/vedro/core/_scenario_discoverer/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_discoverer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_discoverer/_scenario_discoverer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.985702 vedro-1.8.3/vedro/core/_scenario_finder/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.985702 vedro-1.8.3/vedro/core/_scenario_finder/_file_filters/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/_file_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/_file_filters/_any_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/_file_filters/_dunder_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/_file_filters/_ext_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/_file_filters/_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/_file_filters/_hidden_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/_scenario_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_finder/_scenario_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.985702 vedro-1.8.3/vedro/core/_scenario_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_loader/_scenario_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_loader/_scenario_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.985702 vedro-1.8.3/vedro/core/_scenario_orderer/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_orderer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/core/_scenario_result/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_result/_aggregated_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_result/_scenario_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_result/_scenario_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/core/_scenario_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/core/_scenario_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_scenario_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_step_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_virtual_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/_virtual_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/core/scenario_orderer/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_orderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_orderer/_plain_scenario_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_orderer/_scenario_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_orderer/_stable_scenario_orderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/core/scenario_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_runner/_interrupted.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_runner/_monotonic_scenario_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_runner/_scenario_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/core/scenario_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_scheduler/_monotonic_scenario_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/core/scenario_scheduler/_scenario_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/events/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/plugins/artifacted/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/artifacted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/artifacted/_artifacted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.989702 vedro-1.8.3/vedro/plugins/assert_rewriter/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/assert_rewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/assert_rewriter/_assert_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/assert_rewriter/_scenario_assert_rewriter_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.993702 vedro-1.8.3/vedro/plugins/deferrer/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/deferrer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/deferrer/_deferrer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.993702 vedro-1.8.3/vedro/plugins/director/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/_director.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/_director_init_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.993702 vedro-1.8.3/vedro/plugins/director/pycharm/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/pycharm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/pycharm/_pycharm_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.993702 vedro-1.8.3/vedro/plugins/director/rich/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/rich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/rich/_rich_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/rich/_rich_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.993702 vedro-1.8.3/vedro/plugins/director/silent/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/silent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/director/silent/_silent_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.993702 vedro-1.8.3/vedro/plugins/dry_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/dry_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/dry_runner/_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/dry_runner/_dry_runner_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.993702 vedro-1.8.3/vedro/plugins/interrupter/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/interrupter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/interrupter/_interrupter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.997702 vedro-1.8.3/vedro/plugins/orderer/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/orderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/orderer/orderer_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/orderer/random_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/orderer/reversed_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/orderer/stable_orderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.997702 vedro-1.8.3/vedro/plugins/repeater/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/repeater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/repeater/_repeater.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/repeater/_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.997702 vedro-1.8.3/vedro/plugins/rerunner/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/rerunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/rerunner/_rerunner.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/rerunner/_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.997702 vedro-1.8.3/vedro/plugins/seeder/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/seeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/seeder/_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/seeder/_seeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.997702 vedro-1.8.3/vedro/plugins/skipper/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/skipper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/skipper/_only.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/skipper/_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/skipper/_skip_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/skipper/_skipper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.997702 vedro-1.8.3/vedro/plugins/slicer/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/slicer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/slicer/_slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:31.001702 vedro-1.8.3/vedro/plugins/system_upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/system_upgrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/system_upgrade/_system_upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:31.001702 vedro-1.8.3/vedro/plugins/tagger/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/tagger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/tagger/_tagger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:31.001702 vedro-1.8.3/vedro/plugins/terminator/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/terminator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/plugins/terminator/_terminator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:20.000000 vedro-1.8.3/vedro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 08:19:30.981701 vedro-1.8.3/vedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2022-12-04 08:19:30.000000 vedro-1.8.3/vedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2022-12-04 08:19:30.000000 vedro-1.8.3/vedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 08:19:30.000000 vedro-1.8.3/vedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-04 08:19:30.000000 vedro-1.8.3/vedro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-04 08:19:30.000000 vedro-1.8.3/vedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-04 08:19:30.000000 vedro-1.8.3/vedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 18:00:11.000000 vedro-1.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-14 18:00:25.090307 vedro-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-14 18:00:11.000000 vedro-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-14 18:00:25.094307 vedro-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-14 18:00:11.000000 vedro-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.058306 vedro-1.9.0/vedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.058306 vedro-1.9.0/vedro/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/_cmd_arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.062306 vedro-1.9.0/vedro/commands/plugin_command/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/_fetch_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/_get_plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/_install_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/_plugin_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.062306 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.062306 vedro-1.9.0/vedro/commands/run_command/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/run_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/run_command/_run_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.066306 vedro-1.9.0/vedro/commands/version_command/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/version_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/version_command/_version_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.066306 vedro-1.9.0/vedro/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.070306 vedro-1.9.0/vedro/core/_config_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_config_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_config_loader/_config_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_config_loader/_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_config_loader/_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_exc_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.070306 vedro-1.9.0/vedro/core/_module_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_module_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_module_loader/_module_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_module_loader/_module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.070306 vedro-1.9.0/vedro/core/_scenario_discoverer/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_discoverer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_discoverer/_create_vscenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_discoverer/_scenario_discoverer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.070306 vedro-1.9.0/vedro/core/_scenario_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_any_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_dunder_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_ext_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_hidden_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_scenario_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_scenario_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_loader/_scenario_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_loader/_scenario_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_orderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_orderer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_result/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_result/_aggregated_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_result/_scenario_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_result/_scenario_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_virtual_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_virtual_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/core/scenario_orderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_orderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_orderer/_plain_scenario_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_orderer/_scenario_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_orderer/_stable_scenario_orderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/core/scenario_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_runner/_interrupted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_runner/_monotonic_scenario_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_runner/_scenario_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/core/scenario_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_scheduler/_monotonic_scenario_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_scheduler/_scenario_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/plugins/artifacted/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/artifacted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/artifacted/_artifacted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/plugins/assert_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/assert_rewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/assert_rewriter/_assert_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/assert_rewriter/_scenario_assert_rewriter_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/plugins/deferrer/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/deferrer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/deferrer/_deferrer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/director/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/_director.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/_director_init_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/director/pycharm/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/pycharm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/pycharm/_pycharm_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/director/rich/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/rich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/rich/_rich_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/rich/_rich_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/director/silent/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/silent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/silent/_silent_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/dry_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/dry_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/dry_runner/_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/dry_runner/_dry_runner_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/interrupter/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/interrupter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/interrupter/_interrupter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/orderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/orderer_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/random_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/reversed_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/stable_orderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/repeater/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/repeater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/repeater/_repeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/repeater/_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/rerunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/rerunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/rerunner/_rerunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/rerunner/_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/seeder/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/seeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/seeder/_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/seeder/_seeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/skipper/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/_skip_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/_skipper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/vedro/plugins/slicer/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/slicer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/slicer/_slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/vedro/plugins/system_upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/system_upgrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/system_upgrade/_system_upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/vedro/plugins/tagger/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/tagger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/tagger/_tagger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/vedro/plugins/terminator/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/terminator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/terminator/_terminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.058306 vedro-1.9.0/vedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-14 18:00:25.000000 vedro-1.9.0/vedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/top_level.txt
```

### Comparing `vedro-1.8.3/LICENSE.txt` & `vedro-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/PKG-INFO` & `vedro-1.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: vedro
-Version: 1.8.3
+Version: 1.9.0
 Summary: Pragmatic BDD Framework
-Home-page: https://github.com/nikitanovosibirsk/vedro
+Home-page: https://github.com/tsv1/vedro
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/
-Project-URL: GitHub, https://github.com/nikitanovosibirsk/vedro
+Project-URL: GitHub, https://github.com/tsv1/vedro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Vedro
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/vedro/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/vedro)
 [![PyPI](https://img.shields.io/pypi/v/vedro.svg?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro.svg?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 
 (!) Work in progress, **internal** breaking changes (for plugins) are possible until v2.0 is released
 
 ## Installation
```

### Comparing `vedro-1.8.3/README.md` & `vedro-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Vedro
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/vedro/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/vedro)
 [![PyPI](https://img.shields.io/pypi/v/vedro.svg?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro.svg?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 
 (!) Work in progress, **internal** breaking changes (for plugins) are possible until v2.0 is released
 
 ## Installation
```

### Comparing `vedro-1.8.3/setup.cfg` & `vedro-1.9.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.8.3
+current_version = 1.9.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-1.8.3/setup.py` & `vedro-1.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro",
-    version="1.8.3",
+    version="1.9.0",
     description="Pragmatic BDD Framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
-    url="https://github.com/nikitanovosibirsk/vedro",
+    url="https://github.com/tsv1/vedro",
     project_urls={
         "Docs": "https://vedro.io/",
-        "GitHub": "https://github.com/nikitanovosibirsk/vedro",
+        "GitHub": "https://github.com/tsv1/vedro",
     },
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro": ["py.typed"]},
     entry_points={
         "console_scripts": ["vedro = vedro:run"],
     },
```

### Comparing `vedro-1.8.3/vedro/_config.py` & `vedro-1.9.0/vedro/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 )
 from vedro.core.scenario_orderer import StableScenarioOrderer
 
 __all__ = ("Config",)
 
 
 class Config(core.Config):
-
     class Registry(core.Config.Registry):
         Dispatcher = Singleton[Dispatcher](Dispatcher)
 
         ScenarioFinder = Factory[ScenarioFinder](lambda: ScenarioFileFinder(
             file_filter=AnyFilter([HiddenFilter(), DunderFilter(), ExtFilter(only=["py"])]),
             dir_filter=AnyFilter([HiddenFilter(), DunderFilter()])
         ))
```

### Comparing `vedro-1.8.3/vedro/_scenario.py` & `vedro-1.9.0/vedro/_scenario.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             return super().__new__(mcs, name, bases, namespace)
 
         updated_name = "VedroTemplate"
         updated_namespace = {**namespace, "__qualname__": updated_name}
         created = super().__new__(mcs, updated_name, bases, updated_namespace)
 
         cls_globals = getattr(cls_constructor, "__globals__")
-        for idx, (args, kwargs) in enumerate(reversed(cls_params), start=1):
+        for idx, (args, kwargs, decorators) in enumerate(reversed(cls_params), start=1):
             signature = inspect.signature(cls_constructor)  # type: ignore
 
             try:
                 bound_args = signature.bind(None, *args, **kwargs)
             except BaseException as e:
                 module = namespace.get("__module__", "")
                 raise TypeError(f"{e} <{module}.{name}>") from None
@@ -41,15 +41,18 @@
                 "__init__": partialmethod(cls_constructor, *args, **kwargs),
                 "__vedro__template_name__": name,
                 "__vedro__template__": created,
                 "__vedro__template_index__": idx,
                 "__vedro__template_total__": len(cls_params),
                 "__vedro__template_args__": bound_args,
             }
-            cls_globals[cls_name] = type(cls_name, bases, cls_namespace)
+            cls = type(cls_name, bases, cls_namespace)
+            for decorator in decorators:
+                cls = decorator(cls)
+            cls_globals[cls_name] = cls
 
         return created
 
 
 class Scenario(metaclass=_Meta):
     subject: str
```

### Comparing `vedro-1.8.3/vedro/core/__init__.py` & `vedro-1.9.0/vedro/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from ._arg_parser import ArgumentParser
 from ._artifacts import Artifact, FileArtifact, MemoryArtifact
 from ._config_loader import Config, ConfigFileLoader, ConfigLoader, ConfigType, Section
 from ._container import Container, Factory, FactoryType, Singleton
 from ._dispatcher import Dispatcher, Subscriber
 from ._event import Event
 from ._exc_info import ExcInfo
-from ._lifecycle import Lifecycle
 from ._module_loader import ModuleFileLoader, ModuleLoader
 from ._plugin import Plugin, PluginConfig
 from ._report import Report
 from ._scenario_discoverer import MultiScenarioDiscoverer, ScenarioDiscoverer
 from ._scenario_finder import ScenarioFileFinder, ScenarioFinder
 from ._scenario_loader import ScenarioFileLoader, ScenarioLoader
 from ._scenario_result import AggregatedResult, ScenarioResult, ScenarioStatus
 from ._step_result import StepResult, StepStatus
 from ._virtual_scenario import VirtualScenario
 from ._virtual_step import VirtualStep
 from .scenario_orderer import ScenarioOrderer
 from .scenario_runner import MonotonicScenarioRunner, ScenarioRunner
 from .scenario_scheduler import MonotonicScenarioScheduler, ScenarioScheduler
 
-__all__ = ("Dispatcher", "Subscriber", "Event", "ExcInfo", "Lifecycle", "Plugin", "PluginConfig",
+__all__ = ("Dispatcher", "Subscriber", "Event", "ExcInfo", "Plugin", "PluginConfig",
            "Report", "ScenarioRunner", "MonotonicScenarioRunner", "ScenarioDiscoverer",
            "MultiScenarioDiscoverer", "ScenarioFinder", "ScenarioFileFinder", "ScenarioLoader",
            "ScenarioFileLoader", "ScenarioResult", "AggregatedResult", "StepResult",
-           "VirtualScenario", "VirtualStep", "ScenarioStatus", "StepStatus", "ArgumentParser",
+           "VirtualScenario", "VirtualStep", "ScenarioStatus", "StepStatus",
            "ConfigLoader", "ConfigFileLoader", "Config", "Section", "ConfigType",
            "ModuleLoader", "ModuleFileLoader", "Artifact", "MemoryArtifact", "FileArtifact",
            "ScenarioScheduler", "MonotonicScenarioScheduler", "FactoryType",
            "Container", "Factory", "Singleton", "ScenarioOrderer")
```

### Comparing `vedro-1.8.3/vedro/core/_artifacts.py` & `vedro-1.9.0/vedro/core/_artifacts.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_config_loader/_config_file_loader.py` & `vedro-1.9.0/vedro/core/_config_loader/_config_file_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Optional
+from typing import Optional, cast
 
 from .._module_loader import ModuleFileLoader, ModuleLoader
 from ._config_loader import ConfigLoader
 from ._config_type import Config, ConfigType
 
 __all__ = ("ConfigFileLoader",)
 
@@ -15,11 +15,18 @@
         self._module_loader = module_loader or ModuleFileLoader()
 
     async def load(self, path: Path) -> ConfigType:
         if not path.exists():
             return self._default_config
         module = await self._module_loader.load(path)
 
-        config = getattr(module, "Config", self._default_config)
+        config = getattr(module, "Config", None)
+        if config is None:
+            return self._default_config
         assert issubclass(config, Config)
 
-        return config
+        # backward compatibility
+        config.__frozen__ = False
+        config.path = path
+        config.__frozen__ = True
+
+        return cast(ConfigType, config)
```

### Comparing `vedro-1.8.3/vedro/core/_config_loader/_config_type.py` & `vedro-1.9.0/vedro/core/_config_loader/_config_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Any, Type
 
 import cabina
 from cabina import MetaBase
 from cabina.errors import ConfigError
 
 __all__ = ("Config", "Section", "ConfigType",)
@@ -17,14 +18,18 @@
 
 
 class Section(cabina.Section, metaclass=_MetaBase):
     pass
 
 
 class Config(cabina.Config, Section):
+    # Here, we set __file__ as the fallback value for 'path'
+    # However, the actual path will be determined at runtime
+    path: Path = Path(__file__)
+
     class Registry(Section):
         pass
 
     class Plugins(Section):
         pass
```

### Comparing `vedro-1.8.3/vedro/core/_container.py` & `vedro-1.9.0/vedro/core/_container.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_dispatcher.py` & `vedro-1.9.0/vedro/core/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_event.py` & `vedro-1.9.0/vedro/core/_event.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_module_loader/_module_file_loader.py` & `vedro-1.9.0/vedro/core/_module_loader/_module_file_loader.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_plugin.py` & `vedro-1.9.0/vedro/core/_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._config.__name__})"
 
 
 class PluginConfig(Section):
     plugin: Type[Plugin] = Plugin
+    description: str = ""
     enabled: bool = True
```

### Comparing `vedro-1.8.3/vedro/core/_report.py` & `vedro-1.9.0/vedro/core/_report.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py` & `vedro-1.9.0/vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-import inspect
+import warnings
 from pathlib import Path
 from typing import List, Type
 
 from ..._scenario import Scenario
 from .._virtual_scenario import VirtualScenario
 from .._virtual_step import VirtualStep
+from ._create_vscenario import create_vscenario
 from ._scenario_discoverer import ScenarioDiscoverer
 
 __all__ = ("MultiScenarioDiscoverer",)
 
 
 class MultiScenarioDiscoverer(ScenarioDiscoverer):
     def _discover_steps(self, scenario: Type[Scenario]) -> List[VirtualStep]:
-        steps = []
-        for step in scenario.__dict__:
-            if step.startswith("_"):
-                continue
-            method = getattr(scenario, step)
-            if not inspect.isfunction(method):
-                continue
-            steps.append(VirtualStep(method))
-        return steps
+        # child classes may use this method to discover steps
+        warnings.warn("Deprecated: use create_vscenario instead", DeprecationWarning)
+        return create_vscenario(scenario).steps
 
     async def discover(self, root: Path) -> List[VirtualScenario]:
         scenarios = []
         async for path in self._finder.find(root):
             loaded = await self._loader.load(path)
             for scn in loaded:
-                steps = self._discover_steps(scn)
-                scenarios.append(VirtualScenario(scn, steps))
+                scenarios.append(create_vscenario(scn))
         return await self._orderer.sort(scenarios)
```

### Comparing `vedro-1.8.3/vedro/core/_scenario_discoverer/_scenario_discoverer.py` & `vedro-1.9.0/vedro/core/_scenario_discoverer/_scenario_discoverer.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_scenario_finder/_file_filters/_ext_filter.py` & `vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_ext_filter.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_scenario_finder/_scenario_file_finder.py` & `vedro-1.9.0/vedro/core/_scenario_finder/_scenario_file_finder.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_scenario_loader/_scenario_file_loader.py` & `vedro-1.9.0/vedro/core/_scenario_loader/_scenario_file_loader.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_scenario_result/_aggregated_result.py` & `vedro-1.9.0/vedro/core/_scenario_result/_aggregated_result.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_scenario_result/_scenario_result.py` & `vedro-1.9.0/vedro/core/_scenario_result/_scenario_result.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_step_result.py` & `vedro-1.9.0/vedro/core/_step_result.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_virtual_scenario.py` & `vedro-1.9.0/vedro/core/_virtual_scenario.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/_virtual_step.py` & `vedro-1.9.0/vedro/core/_virtual_step.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/scenario_orderer/_stable_scenario_orderer.py` & `vedro-1.9.0/vedro/core/scenario_orderer/_stable_scenario_orderer.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/scenario_runner/_interrupted.py` & `vedro-1.9.0/vedro/core/scenario_runner/_interrupted.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/scenario_runner/_monotonic_scenario_runner.py` & `vedro-1.9.0/vedro/core/scenario_runner/_monotonic_scenario_runner.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/scenario_scheduler/_monotonic_scenario_scheduler.py` & `vedro-1.9.0/vedro/core/scenario_scheduler/_monotonic_scenario_scheduler.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/core/scenario_scheduler/_scenario_scheduler.py` & `vedro-1.9.0/vedro/core/scenario_scheduler/_scenario_scheduler.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/events/__init__.py` & `vedro-1.9.0/vedro/events/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import warnings
-from argparse import Namespace
+from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from typing import List
 
-from ..core._arg_parser import ArgumentParser
 from ..core._config_loader import ConfigType
 from ..core._event import Event
 from ..core._exc_info import ExcInfo
 from ..core._report import Report
 from ..core._scenario_result import AggregatedResult, ScenarioResult
 from ..core._step_result import StepResult
 from ..core._virtual_scenario import VirtualScenario
@@ -61,15 +60,15 @@
 
     @property
     def scheduler(self) -> ScenarioScheduler:
         return self._scheduler
 
     @property
     def scenarios(self) -> List[VirtualScenario]:
-        warnings.warn("Deprecated: use scheduler.scenarios instead", DeprecationWarning)
+        warnings.warn("Deprecated: use scheduler.discovered instead", DeprecationWarning)
         return list(self._scheduler.discovered)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._scheduler!r})"
 
 
 class _ScenarioEvent(Event):
```

### Comparing `vedro-1.8.3/vedro/plugins/artifacted/_artifacted.py` & `vedro-1.9.0/vedro/plugins/artifacted/_artifacted.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,7 +59,8 @@
         while len(self._scenario_artifacts) > 0:
             artifact = self._scenario_artifacts.popleft()
             event.scenario_result.attach(artifact)
 
 
 class Artifacted(PluginConfig):
     plugin = ArtifactedPlugin
+    description = "Manages artifacts for step and scenario results"
```

### Comparing `vedro-1.8.3/vedro/plugins/assert_rewriter/_assert_rewriter.py` & `vedro-1.9.0/vedro/plugins/assert_rewriter/_assert_rewriter.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,7 +28,8 @@
 
         self._global_config.Registry.ScenarioLoader.register(
             lambda: ScenarioAssertRewriterLoader(AssertionRewritingHook()), self)
 
 
 class AssertRewriter(PluginConfig):
     plugin = AssertRewriterPlugin
+    description = "Rewrites assert statements to provide better error messages"
```

### Comparing `vedro-1.8.3/vedro/plugins/deferrer/_deferrer.py` & `vedro-1.9.0/vedro/plugins/deferrer/_deferrer.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,7 +38,8 @@
                 await fn(*args, **kwargs)
             else:
                 fn(*args, **kwargs)
 
 
 class Deferrer(PluginConfig):
     plugin = DeferrerPlugin
+    description = "Executes deferred functions at the end of each scenario"
```

### Comparing `vedro-1.8.3/vedro/plugins/director/__init__.py` & `vedro-1.9.0/vedro/plugins/director/__init__.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/director/_director.py` & `vedro-1.9.0/vedro/plugins/director/_director.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,7 +39,8 @@
         if len(self._reporters) == 0:
             self._default_reporter = name
         self._reporters[name] = reporter
 
 
 class Director(PluginConfig):
     plugin = DirectorPlugin
+    description = "Manages and configures reporters for scenario execution"
```

### Comparing `vedro-1.8.3/vedro/plugins/director/_director_init_event.py` & `vedro-1.9.0/vedro/plugins/director/_director_init_event.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/director/pycharm/_pycharm_reporter.py` & `vedro-1.9.0/vedro/plugins/director/pycharm/_pycharm_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
             message += f" {key}='{escaped}'"
         message += "]"
         self._printer.console.out(message)
 
 
 class PyCharmReporter(PluginConfig):
     plugin = PyCharmReporterPlugin
+    description = "Outputs scenario results in a PyCharm-friendly format"
 
     # Show internal calls in the traceback output
     show_internal_calls: bool = False
 
     # Show skipped scenarios
     show_skipped: bool = True
```

### Comparing `vedro-1.8.3/vedro/plugins/director/rich/_rich_printer.py` & `vedro-1.9.0/vedro/plugins/director/rich/_rich_printer.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             style = Style(color="grey70")
         else:
             return
 
         self._console.out(prefix, end="")
         if elapsed is not None:
             self._console.out(subject, style=style, end="")
-            self._console.out(f" ({elapsed:.2f}s)", style=Style(color="grey50"))
+            self._console.out(f" ({self.format_elapsed(elapsed)})", style=Style(color="grey50"))
         else:
             self._console.out(subject, style=style)
 
     def print_scenario_caption(self, caption: str, *, prefix: str = "") -> None:
         self._console.out(prefix, end="")
         self._console.out(f"{caption}", style=Style(color="grey50"))
 
@@ -72,15 +72,15 @@
             style = Style(color="red")
         else:
             return
 
         self._console.out(prefix, end="")
         if elapsed is not None:
             self._console.out(name, style=style, end="")
-            self._console.out(f" ({elapsed:.2f}s)", style=Style(color="grey50"))
+            self._console.out(f" ({self.format_elapsed(elapsed)})", style=Style(color="grey50"))
         else:
             self._console.out(name, style=style)
 
     def __filter_internals(self, traceback: TracebackType) -> TracebackType:
         class _Traceback:
             def __init__(self, tb_frame: FrameType, tb_lasti: int, tb_lineno: int,
                          tb_next: Optional[TracebackType]) -> None:
@@ -112,15 +112,15 @@
         self._console.out("".join(formatted), style=Style(color="yellow"))
 
     def __filter_locals(self, trace: Trace) -> None:
         for stack in trace.stacks:
             for frame in stack.frames:
                 if frame.locals is not None:
                     frame.locals = {k: v for k, v in frame.locals.items()
-                                    if k != "self" and not k.startswith("@")}
+                                    if k != "self" and k.isidentifier()}
 
     def print_pretty_exception(self, exc_info: ExcInfo, *,
                                max_frames: int = 8,  # min=4 (see rich.traceback.Traceback impl)
                                show_locals: bool = False,
                                show_internal_calls: bool = False,
                                word_wrap: bool = False) -> None:
         if show_internal_calls:
@@ -176,26 +176,38 @@
 
     def print_report_summary(self, summary: List[str]) -> None:
         if len(summary) == 0:
             return
         text = "# " + "\n# ".join(summary)
         self._console.out(text, style=Style(color="grey70"))
 
+    def format_elapsed(self, elapsed: float) -> str:
+        hours = int(elapsed // 3600)
+        minutes = int((elapsed - hours * 3600) // 60)
+        seconds = elapsed - hours * 3600 - minutes * 60
+
+        formatted = f"{seconds:.2f}s" if elapsed < 60 else f"{int(seconds)}s"
+        if (minutes > 0) or (hours > 0):
+            formatted = f"{minutes}m {formatted}"
+        if hours > 0:
+            formatted = f"{hours}h {formatted}"
+        return formatted
+
     def print_report_stats(self, *, total: int, passed: int, failed: int, skipped: int,
                            elapsed: float, is_interrupted: bool = False) -> None:
         if is_interrupted or (failed > 0 or passed == 0):
             style = Style(color="red", bold=True)
         else:
             style = Style(color="green", bold=True)
 
         scenarios = "scenario" if (total == 1) else "scenarios"
         self._console.out(f"# {total} {scenarios}, "
                           f"{passed} passed, {failed} failed, {skipped} skipped",
                           style=style, end="")
-        self._console.out(f" ({elapsed:.2f}s)", style=Style(color="blue"))
+        self._console.out(f" ({self.format_elapsed(elapsed)})", style=Style(color="blue"))
 
     def print_empty_line(self) -> None:
         self._console.out(" ")
 
     def print(self, smth: Any, *, end: str = "\n") -> None:
         self._console.out(smth, end=end)
```

### Comparing `vedro-1.8.3/vedro/plugins/director/rich/_rich_reporter.py` & `vedro-1.9.0/vedro/plugins/director/rich/_rich_reporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,17 +27,19 @@
         self._tb_pretty = config.tb_pretty
         self._tb_show_internal_calls = config.tb_show_internal_calls
         self._tb_show_locals = config.tb_show_locals
         self._tb_max_frames = config.tb_max_frames
         self._show_skipped = config.show_skipped
         self._show_timings = config.show_timings
         self._show_paths = config.show_paths
+        self._show_steps = config.show_steps
         self._hide_namespaces = config.hide_namespaces
         self._show_scenario_spinner = config.show_scenario_spinner
         self._show_interrupted_traceback = config.show_interrupted_traceback
+        self._v2_verbosity = config.v2_verbosity
         self._namespace: Union[str, None] = None
 
     def subscribe(self, dispatcher: Dispatcher) -> None:
         super().subscribe(dispatcher)
         dispatcher.listen(DirectorInitEvent, lambda e: e.director.register("rich", self))
 
     def on_chosen(self) -> None:
@@ -60,14 +62,18 @@
                            action="count",
                            default=self._verbosity,
                            help=help_message)
         group.add_argument("--show-timings",
                            action="store_true",
                            default=self._show_timings,
                            help="Show the elapsed time of each scenario")
+        group.add_argument("--show-steps",
+                           action="store_true",
+                           default=self._show_steps,
+                           help="Show scenario step names")
         group.add_argument("--show-paths",
                            action="store_true",
                            default=self._show_paths,
                            help="Show the relative path of each passed scenario")
         group.add_argument("--hide-namespaces",
                            action="store_true",
                            default=self._hide_namespaces,
@@ -79,16 +85,19 @@
         group.add_argument("--tb-show-locals",
                            action="store_true",
                            default=self._tb_show_locals,
                            help="Show local variables in the traceback output")
 
     def on_arg_parsed(self, event: ArgParsedEvent) -> None:
         self._verbosity = event.args.verbose
+        if self._v2_verbosity:
+            self._verbosity = self._verbosity + 2
         self._show_timings = event.args.show_timings
         self._show_paths = event.args.show_paths
+        self._show_steps = event.args.show_steps
         self._hide_namespaces = event.args.hide_namespaces
         self._tb_show_internal_calls = event.args.tb_show_internal_calls
         self._tb_show_locals = event.args.tb_show_locals
 
         assert self._tb_max_frames >= 4, \
             "RichReporter: `max_frames` must be >= 4"
 
@@ -135,14 +144,20 @@
 
     def _print_scenario_passed(self, scenario_result: ScenarioResult, *, prefix: str = "") -> None:
         elapsed = scenario_result.elapsed if self._show_timings else None
         self._printer.print_scenario_subject(scenario_result.scenario.subject,
                                              scenario_result.status,
                                              elapsed=elapsed,
                                              prefix=prefix)
+        if self._show_steps:
+            for step_result in scenario_result.step_results:
+                elapsed = step_result.elapsed if self._show_timings else None
+                step_prefix = self._prefix_to_indent(prefix, indent=2)
+                self._printer.print_step_name(step_result.step_name, step_result.status,
+                                              elapsed=elapsed, prefix=step_prefix)
 
         if self._show_paths:
             caption = f"> {scenario_result.scenario.rel_path}"
             caption_prefix = self._prefix_to_indent(prefix, indent=2)
             self._printer.print_scenario_caption(caption, prefix=caption_prefix)
 
     def _print_scenario_failed(self, scenario_result: ScenarioResult, *, prefix: str = "") -> None:
@@ -220,24 +235,28 @@
                                          skipped=event.report.skipped,
                                          elapsed=event.report.elapsed,
                                          is_interrupted=is_interrupted)
 
 
 class RichReporter(PluginConfig):
     plugin = RichReporterPlugin
+    description = "Enhanced, customizable scenario reporting with rich output"
 
     # Show skipped scenarios
     show_skipped: bool = True
 
     # Show the elapsed time of each scenario
     show_timings: bool = False
 
     # Show the relative path of each passed scenario
     show_paths: bool = False
 
+    # Show scenario step names
+    show_steps: bool = False
+
     # Don't show scenario namespaces
     hide_namespaces: bool = False
 
     # Show status indicator of the current running scenario
     show_scenario_spinner: bool = False
 
     # Show pretty traceback
@@ -251,7 +270,10 @@
     tb_show_locals: bool = False
 
     # Max stack trace entries to show (min=4)
     tb_max_frames: int = 8
 
     # Show traceback if the execution is interrupted
     show_interrupted_traceback: bool = False
+
+    # Enable new verbose levels
+    v2_verbosity: bool = False
```

### Comparing `vedro-1.8.3/vedro/plugins/dry_runner/_dry_runner.py` & `vedro-1.9.0/vedro/plugins/dry_runner/_dry_runner.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/dry_runner/_dry_runner_plugin.py` & `vedro-1.9.0/vedro/plugins/dry_runner/_dry_runner_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,10 +33,11 @@
                                                interrupt_exceptions=self._interrupt_exceptions),
                 registrant=self
             )
 
 
 class DryRunner(PluginConfig):
     plugin = DryRunnerPlugin
+    description = "Simulates scenario execution without actually executing them"
 
     # Exceptions that will interrupt scenario execution
     interrupt_exceptions: Tuple[Type[BaseException], ...] = (KeyboardInterrupt, SystemExit,)
```

### Comparing `vedro-1.8.3/vedro/plugins/interrupter/_interrupter.py` & `vedro-1.9.0/vedro/plugins/interrupter/_interrupter.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,10 +77,11 @@
         for sig, orig_handler in self._orig_handlers.items():
             signal.signal(sig, orig_handler)
         self._orig_handlers = {}
 
 
 class Interrupter(PluginConfig):
     plugin = InterrupterPlugin
+    description = "Stops test execution after the first failed scenario or on specified signals"
 
     # Raise Interrupted exception on these signals
     handle_signals: Tuple[signal.Signals, ...] = (signal.SIGTERM,)
```

### Comparing `vedro-1.8.3/vedro/plugins/orderer/orderer_plugin.py` & `vedro-1.9.0/vedro/plugins/orderer/orderer_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,7 +39,8 @@
 
         if event.args.order_stable:
             self._global_config.Registry.ScenarioOrderer.register(StableScenarioOrderer, self)
 
 
 class Orderer(PluginConfig):
     plugin = OrdererPlugin
+    description = "Configures the execution order of scenarios"
```

### Comparing `vedro-1.8.3/vedro/plugins/repeater/_repeater.py` & `vedro-1.9.0/vedro/plugins/repeater/_repeater.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,7 +70,8 @@
     def on_cleanup(self, event: CleanupEvent) -> None:
         if self._repeats > 1:
             event.report.add_summary(f"repeated x{self._repeats}")
 
 
 class Repeater(PluginConfig):
     plugin = RepeaterPlugin
+    description = "Repeat scenarios a specified number of times"
```

### Comparing `vedro-1.8.3/vedro/plugins/repeater/_scheduler.py` & `vedro-1.9.0/vedro/plugins/repeater/_scheduler.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/rerunner/_rerunner.py` & `vedro-1.9.0/vedro/plugins/rerunner/_rerunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,7 +77,8 @@
             ss = "" if self._reran == 1 else "s"
             ts = "" if self._times == 1 else "s"
             event.report.add_summary(f"rerun {self._reran} scenario{ss}, {self._times} time{ts}")
 
 
 class Rerunner(PluginConfig):
     plugin = RerunnerPlugin
+    description = "Reruns failed scenarios a specified number of times"
```

### Comparing `vedro-1.8.3/vedro/plugins/rerunner/_scheduler.py` & `vedro-1.9.0/vedro/plugins/rerunner/_scheduler.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/seeder/_random.py` & `vedro-1.9.0/vedro/plugins/seeder/_random.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/seeder/_seeder.py` & `vedro-1.9.0/vedro/plugins/seeder/_seeder.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,7 +85,8 @@
     def on_cleanup(self, event: CleanupEvent) -> None:
         if (event.report.passed + event.report.failed) > 0:
             event.report.add_summary(f"--seed {self._inital_seed}")
 
 
 class Seeder(PluginConfig):
     plugin = SeederPlugin
+    description = "Sets seeds for deterministic random behavior in scenarios"
```

### Comparing `vedro-1.8.3/vedro/plugins/skipper/_only.py` & `vedro-1.9.0/vedro/plugins/skipper/_only.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/skipper/_skip.py` & `vedro-1.9.0/vedro/plugins/skipper/_skip.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/skipper/_skip_if.py` & `vedro-1.9.0/vedro/plugins/skipper/_skip_if.py`

 * *Files identical despite different names*

### Comparing `vedro-1.8.3/vedro/plugins/skipper/_skipper.py` & `vedro-1.9.0/vedro/plugins/skipper/_skipper.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,21 +63,31 @@
         path = os.path.normpath(file_or_dir)
         if os.path.isabs(path):
             return path
         if os.path.commonpath(["scenarios", path]) != "scenarios":
             path = os.path.join("scenarios", path)
         return os.path.abspath(path)
 
+    def _get_scenario_attr(self, scenario: VirtualScenario, attr: str) -> bool:
+        template = getattr(scenario._orig_scenario, "__vedro__template__", None)
+        return getattr(template or scenario._orig_scenario, attr, False)
+
     def _is_scenario_skipped(self, scenario: VirtualScenario) -> bool:
+        attr_name = "__vedro__skipped__"
         template = getattr(scenario._orig_scenario, "__vedro__template__", None)
-        return getattr(template or scenario._orig_scenario, "__vedro__skipped__", False)
+        if template and hasattr(template, attr_name):
+            return bool(getattr(template, attr_name))
+        return getattr(scenario._orig_scenario, attr_name, False)
 
     def _is_scenario_special(self, scenario: VirtualScenario) -> bool:
+        attr_name = "__vedro__only__"
         template = getattr(scenario._orig_scenario, "__vedro__template__", None)
-        return getattr(template or scenario._orig_scenario, "__vedro__only__", False)
+        if template and hasattr(template, attr_name):
+            return bool(getattr(template, attr_name))
+        return getattr(scenario._orig_scenario, attr_name, False)
 
     def _is_match_scenario(self, path: _CompositePath, scenario: VirtualScenario) -> bool:
         if os.path.commonpath([path.file_path, scenario.path]) != path.file_path:
             return False
 
         if (path.cls_name is not None) and (path.cls_name != scenario.name):
             return False
@@ -128,7 +138,9 @@
             async for scenario in scheduler:
                 if scenario.unique_id not in special_scenarios:
                     scheduler.ignore(scenario)
 
 
 class Skipper(PluginConfig):
     plugin = SkipperPlugin
+    description = "Allows selective scenario skipping and selection " \
+                  "based on file/directory or subject"
```

### Comparing `vedro-1.8.3/vedro/plugins/slicer/_slicer.py` & `vedro-1.9.0/vedro/plugins/slicer/_slicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,7 +46,8 @@
                 if (index % self._total) != self._index:
                     event.scheduler.ignore(scenario)
                 index += 1
 
 
 class Slicer(PluginConfig):
     plugin = SlicerPlugin
+    description = "Provides a way to distribute scenarios among multiple workers"
```

### Comparing `vedro-1.8.3/vedro/plugins/system_upgrade/_system_upgrade.py` & `vedro-1.9.0/vedro/plugins/system_upgrade/_system_upgrade.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def _get_user_agent(self) -> str:
         python_version = platform.python_version()
         platform_info = platform.platform(terse=True)
         return f"Vedro/{self._cur_version} (Python/{python_version}; {platform_info})"
 
     def _get_latest_version(self) -> None:
-        url = f"{self._api_url}/v1/last-version"
+        url = f"{self._api_url}/v1/latest-version"
         headers = {"User-Agent": self._get_user_agent()}
         response = self._send_request(url, headers=headers, timeout=self._timeout)
         if isinstance(response, dict) and ("version" in response):
             self._latest_version = response["version"]
 
     def on_startup(self, event: StartupEvent) -> None:
         self._thread = Thread(target=self._get_latest_version, daemon=True)
@@ -68,13 +68,14 @@
         if not self._is_up_to_date(self._cur_version, self._latest_version):
             message = f"(!) Vedro update available: {self._cur_version} → {self._latest_version}"
             event.report.add_summary(message)
 
 
 class SystemUpgrade(PluginConfig):
     plugin = SystemUpgradePlugin
+    description = "Checks for Vedro updates and notifies when a newer version is available"
 
     # URL to the Vedro API
     api_url: str = "https://api.vedro.io"
 
     # Timeout for the request to the API
     timeout: float = 1.0
```

### Comparing `vedro-1.8.3/vedro/plugins/terminator/_terminator.py` & `vedro-1.9.0/vedro/plugins/terminator/_terminator.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,18 +15,19 @@
     def subscribe(self, dispatcher: Dispatcher) -> None:
         dispatcher.listen(CleanupEvent, self.on_cleanup, priority=sys.maxsize)
 
     def on_cleanup(self, event: CleanupEvent) -> None:
         if event.report.interrupted:
             exc = event.report.interrupted.value
             if isinstance(exc, SystemExit) and (exc.code is not None):
-                self._exit_fn(exc.code)
+                self._exit_fn(int(exc.code))
             else:
                 self._exit_fn(130)
         elif event.report.failed > 0 or event.report.passed == 0:
             self._exit_fn(1)
         else:
             self._exit_fn(0)
 
 
 class Terminator(PluginConfig):
     plugin = TerminatorPlugin
+    description = "Handles test exit status based on test results and interruptions"
```

### Comparing `vedro-1.8.3/vedro.egg-info/PKG-INFO` & `vedro-1.9.0/vedro.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: vedro
-Version: 1.8.3
+Version: 1.9.0
 Summary: Pragmatic BDD Framework
-Home-page: https://github.com/nikitanovosibirsk/vedro
+Home-page: https://github.com/tsv1/vedro
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/
-Project-URL: GitHub, https://github.com/nikitanovosibirsk/vedro
+Project-URL: GitHub, https://github.com/tsv1/vedro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Vedro
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/vedro/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/vedro)
 [![PyPI](https://img.shields.io/pypi/v/vedro.svg?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro.svg?style=flat-square)](https://pypi.python.org/pypi/vedro/)
 
 (!) Work in progress, **internal** breaking changes (for plugins) are possible until v2.0 is released
 
 ## Installation
```

### Comparing `vedro-1.8.3/vedro.egg-info/SOURCES.txt` & `vedro-1.9.0/vedro.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,45 +3,63 @@
 setup.cfg
 setup.py
 vedro/__init__.py
 vedro/__main__.py
 vedro/_config.py
 vedro/_context.py
 vedro/_interface.py
+vedro/_main.py
 vedro/_params.py
 vedro/_scenario.py
 vedro/_version.py
 vedro/py.typed
 vedro.egg-info/PKG-INFO
 vedro.egg-info/SOURCES.txt
 vedro.egg-info/dependency_links.txt
 vedro.egg-info/entry_points.txt
 vedro.egg-info/requires.txt
 vedro.egg-info/top_level.txt
+vedro/commands/__init__.py
+vedro/commands/_cmd_arg_parser.py
+vedro/commands/_command.py
+vedro/commands/plugin_command/__init__.py
+vedro/commands/plugin_command/_fetch_plugins.py
+vedro/commands/plugin_command/_get_plugin_info.py
+vedro/commands/plugin_command/_install_plugin.py
+vedro/commands/plugin_command/_plugin_command.py
+vedro/commands/plugin_command/plugin_manager/__init__.py
+vedro/commands/plugin_command/plugin_manager/_config_generator.py
+vedro/commands/plugin_command/plugin_manager/_config_markup.py
+vedro/commands/plugin_command/plugin_manager/_config_parser.py
+vedro/commands/plugin_command/plugin_manager/_config_updater.py
+vedro/commands/plugin_command/plugin_manager/_plugin_manager.py
+vedro/commands/run_command/__init__.py
+vedro/commands/run_command/_run_command.py
+vedro/commands/version_command/__init__.py
+vedro/commands/version_command/_version_command.py
 vedro/core/__init__.py
-vedro/core/_arg_parser.py
 vedro/core/_artifacts.py
 vedro/core/_container.py
 vedro/core/_dispatcher.py
 vedro/core/_event.py
 vedro/core/_exc_info.py
-vedro/core/_lifecycle.py
 vedro/core/_plugin.py
 vedro/core/_report.py
 vedro/core/_step_result.py
 vedro/core/_virtual_scenario.py
 vedro/core/_virtual_step.py
 vedro/core/_config_loader/__init__.py
 vedro/core/_config_loader/_config_file_loader.py
 vedro/core/_config_loader/_config_loader.py
 vedro/core/_config_loader/_config_type.py
 vedro/core/_module_loader/__init__.py
 vedro/core/_module_loader/_module_file_loader.py
 vedro/core/_module_loader/_module_loader.py
 vedro/core/_scenario_discoverer/__init__.py
+vedro/core/_scenario_discoverer/_create_vscenario.py
 vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py
 vedro/core/_scenario_discoverer/_scenario_discoverer.py
 vedro/core/_scenario_finder/__init__.py
 vedro/core/_scenario_finder/_scenario_file_finder.py
 vedro/core/_scenario_finder/_scenario_finder.py
 vedro/core/_scenario_finder/_file_filters/__init__.py
 vedro/core/_scenario_finder/_file_filters/_any_filter.py
```

