# Comparing `tmp/CADET-Process-0.7.0.tar.gz` & `tmp/CADET-Process-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CADET-Process-0.7.0.tar", last modified: Fri Mar 24 16:14:19 2023, max compression
+gzip compressed data, was "CADET-Process-0.7.1.tar", last modified: Sun May 14 12:49:46 2023, max compression
```

## Comparing `CADET-Process-0.7.0.tar` & `CADET-Process-0.7.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.124720 CADET-Process-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.112720 CADET-Process-0.7.0/CADETProcess/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/CADETProcessError.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.112720 CADET-Process-0.7.0/CADETProcess/comparison/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/comparison/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)    29078 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/comparison/difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/comparison/peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/comparison/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.112720 CADET-Process-0.7.0/CADETProcess/dataStructure/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dataStructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dataStructure/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dataStructure/dataStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dataStructure/diskcache.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dataStructure/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dataStructure/nested_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    16173 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dataStructure/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dataStructure/parameter_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.112720 CADET-Process-0.7.0/CADETProcess/dynamicEvents/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dynamicEvents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dynamicEvents/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/dynamicEvents/section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.116720 CADET-Process-0.7.0/CADETProcess/equilibria/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/equilibria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/equilibria/buffer_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/equilibria/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/equilibria/ptc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/equilibria/reaction_equilibria.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.116720 CADET-Process-0.7.0/CADETProcess/fractionation/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/fractionation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/fractionation/fractionationOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/fractionation/fractionator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/fractionation/fractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.116720 CADET-Process-0.7.0/CADETProcess/modelBuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/modelBuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/modelBuilder/carouselBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/modelBuilder/compartmentBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.116720 CADET-Process-0.7.0/CADETProcess/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/individual.py
--rw-r--r--   0 runner    (1001) docker     (123)    98472 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/optimizationProblem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/population.py
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/pymooAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/optimization/scipyAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.116720 CADET-Process-0.7.0/CADETProcess/processModel/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40505 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/componentSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/discretization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31594 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/flowSheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/process.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26945 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/solutionRecorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    34406 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/processModel/unitOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/simulationResults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.120720 CADET-Process-0.7.0/CADETProcess/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54643 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/simulator/cadetAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/simulator/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/smoothing2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48807 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/stationarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.120720 CADET-Process-0.7.0/CADETProcess/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/tools/yamamoto.py
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/CADETProcess/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.120720 CADET-Process-0.7.0/CADET_Process.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-03-24 16:14:19.000000 CADET-Process-0.7.0/CADET_Process.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-24 16:14:19.000000 CADET-Process-0.7.0/CADET_Process.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:14:19.000000 CADET-Process-0.7.0/CADET_Process.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-24 16:14:19.000000 CADET-Process-0.7.0/CADET_Process.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 16:14:19.000000 CADET-Process-0.7.0/CADET_Process.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-03-24 16:14:19.124720 CADET-Process-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.120720 CADET-Process-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.120720 CADET-Process-0.7.0/examples/batch_elution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/batch_elution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/batch_elution/optimization_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/batch_elution/optimization_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/batch_elution/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.120720 CADET-Process-0.7.0/examples/characterize_chromatographic_system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/characterize_chromatographic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/characterize_chromatographic_system/binding_model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/characterize_chromatographic_system/column_transport_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/characterize_chromatographic_system/particle_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/characterize_chromatographic_system/system_periphery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.120720 CADET-Process-0.7.0/examples/load_wash_elute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/load_wash_elute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/load_wash_elute/lwe_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/load_wash_elute/lwe_flow_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.120720 CADET-Process-0.7.0/examples/recycling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/recycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/recycling/clr_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/examples/recycling/mrssr_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-24 16:14:19.124720 CADET-Process-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:19.124720 CADET-Process-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_buffer_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_carousel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_compartment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_flow_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_fractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_individual.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_optimization_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_optimization_results.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5624 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_population.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)    19066 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-03-24 16:14:10.000000 CADET-Process-0.7.0/tests/test_unit_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.163083 CADET-Process-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.143083 CADET-Process-0.7.1/CADETProcess/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/CADETProcessError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.143083 CADET-Process-0.7.1/CADETProcess/comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29078 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.143083 CADET-Process-0.7.1/CADETProcess/dataStructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/dataStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/diskcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/nested_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16173 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/parameter_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.147083 CADET-Process-0.7.1/CADETProcess/dynamicEvents/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dynamicEvents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dynamicEvents/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dynamicEvents/section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.147083 CADET-Process-0.7.1/CADETProcess/equilibria/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/buffer_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/ptc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/reaction_equilibria.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.147083 CADET-Process-0.7.1/CADETProcess/fractionation/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/fractionation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/fractionation/fractionationOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/fractionation/fractionator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/fractionation/fractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.147083 CADET-Process-0.7.1/CADETProcess/modelBuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/modelBuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/modelBuilder/carouselBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/modelBuilder/compartmentBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.151083 CADET-Process-0.7.1/CADETProcess/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98472 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/optimizationProblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/pymooAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/scipyAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.151083 CADET-Process-0.7.1/CADETProcess/processModel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40569 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/componentSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/flowSheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/process.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26945 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/solutionRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34406 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/unitOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/simulationResults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/CADETProcess/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54643 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/simulator/cadetAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/simulator/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/smoothing2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48809 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/stationarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/CADETProcess/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/tools/yamamoto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/CADET_Process.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-14 12:49:46.163083 CADET-Process-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/examples/batch_elution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/batch_elution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/batch_elution/optimization_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/batch_elution/optimization_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/batch_elution/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/examples/characterize_chromatographic_system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/binding_model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/column_transport_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/particle_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/system_periphery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/examples/load_wash_elute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/load_wash_elute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/load_wash_elute/lwe_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/load_wash_elute/lwe_flow_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.159083 CADET-Process-0.7.1/examples/recycling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/recycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/recycling/clr_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/recycling/mrssr_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-14 12:49:46.163083 CADET-Process-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.163083 CADET-Process-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_buffer_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_carousel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_flow_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_fractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_optimization_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_optimization_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5624 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19066 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_unit_operation.py
```

### Comparing `CADET-Process-0.7.0/CADETProcess/__init__.py` & `CADET-Process-0.7.1/CADETProcess/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 advanced chromatographic systems. It serves as an inteface for CADET, but also
 for other solvers.
 
 See https://cadet-process.readthedocs.io for complete documentation.
 """
 # Version information
 name = 'CADET-Process'
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 # Imports
 from .CADETProcessError import *
 
 from . import log
 
 from .settings import Settings
```

### Comparing `CADET-Process-0.7.0/CADETProcess/comparison/__init__.py` & `CADET-Process-0.7.1/CADETProcess/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/comparison/comparator.py` & `CADET-Process-0.7.1/CADETProcess/comparison/comparator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/comparison/difference.py` & `CADET-Process-0.7.1/CADETProcess/comparison/difference.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/comparison/peaks.py` & `CADET-Process-0.7.1/CADETProcess/comparison/peaks.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/comparison/shape.py` & `CADET-Process-0.7.1/CADETProcess/comparison/shape.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dataStructure/__init__.py` & `CADET-Process-0.7.1/CADETProcess/dataStructure/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dataStructure/cache.py` & `CADET-Process-0.7.1/CADETProcess/dataStructure/cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dataStructure/dataStructure.py` & `CADET-Process-0.7.1/CADETProcess/dataStructure/dataStructure.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dataStructure/diskcache.py` & `CADET-Process-0.7.1/CADETProcess/dataStructure/diskcache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dataStructure/nested_dict.py` & `CADET-Process-0.7.1/CADETProcess/dataStructure/nested_dict.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dataStructure/parameter.py` & `CADET-Process-0.7.1/CADETProcess/dataStructure/parameter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dataStructure/parameter_group.py` & `CADET-Process-0.7.1/CADETProcess/dataStructure/parameter_group.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dynamicEvents/__init__.py` & `CADET-Process-0.7.1/CADETProcess/dynamicEvents/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dynamicEvents/event.py` & `CADET-Process-0.7.1/CADETProcess/dynamicEvents/event.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/dynamicEvents/section.py` & `CADET-Process-0.7.1/CADETProcess/dynamicEvents/section.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/equilibria/__init__.py` & `CADET-Process-0.7.1/CADETProcess/equilibria/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/equilibria/buffer_capacity.py` & `CADET-Process-0.7.1/CADETProcess/equilibria/buffer_capacity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/equilibria/initial_conditions.py` & `CADET-Process-0.7.1/CADETProcess/equilibria/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/equilibria/ptc.py` & `CADET-Process-0.7.1/CADETProcess/equilibria/ptc.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/equilibria/reaction_equilibria.py` & `CADET-Process-0.7.1/CADETProcess/equilibria/reaction_equilibria.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/fractionation/fractionationOptimizer.py` & `CADET-Process-0.7.1/CADETProcess/fractionation/fractionationOptimizer.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/fractionation/fractionator.py` & `CADET-Process-0.7.1/CADETProcess/fractionation/fractionator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/fractionation/fractions.py` & `CADET-Process-0.7.1/CADETProcess/fractionation/fractions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/log.py` & `CADET-Process-0.7.1/CADETProcess/log.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/modelBuilder/__init__.py` & `CADET-Process-0.7.1/CADETProcess/modelBuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/modelBuilder/carouselBuilder.py` & `CADET-Process-0.7.1/CADETProcess/modelBuilder/carouselBuilder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/modelBuilder/compartmentBuilder.py` & `CADET-Process-0.7.1/CADETProcess/modelBuilder/compartmentBuilder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/__init__.py` & `CADET-Process-0.7.1/CADETProcess/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/cache.py` & `CADET-Process-0.7.1/CADETProcess/optimization/cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/individual.py` & `CADET-Process-0.7.1/CADETProcess/optimization/individual.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/optimizationProblem.py` & `CADET-Process-0.7.1/CADETProcess/optimization/optimizationProblem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/optimizer.py` & `CADET-Process-0.7.1/CADETProcess/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/population.py` & `CADET-Process-0.7.1/CADETProcess/optimization/population.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/pymooAdapter.py` & `CADET-Process-0.7.1/CADETProcess/optimization/pymooAdapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/results.py` & `CADET-Process-0.7.1/CADETProcess/optimization/results.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/optimization/scipyAdapter.py` & `CADET-Process-0.7.1/CADETProcess/optimization/scipyAdapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/performance.py` & `CADET-Process-0.7.1/CADETProcess/performance.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/plotting.py` & `CADET-Process-0.7.1/CADETProcess/plotting.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/__init__.py` & `CADET-Process-0.7.1/CADETProcess/processModel/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/binding.py` & `CADET-Process-0.7.1/CADETProcess/processModel/binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     'LangmuirLDF',
     'BiLangmuir',
     'BiLangmuirLDF',
     'FreundlichLDF',
     'StericMassAction',
     'AntiLangmuir',
     'Spreading',
+    'MobilePhaseModulator',
+    'ExtendedMobilePhaseModulator',
     'SelfAssociation',
     'BiStericMassAction',
     'MultistateStericMassAction',
     'SimplifiedMultistateStericMassAction',
     'Saska',
     'GeneralizedIonExchange',
 ]
```

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/componentSystem.py` & `CADET-Process-0.7.1/CADETProcess/processModel/componentSystem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/discretization.py` & `CADET-Process-0.7.1/CADETProcess/processModel/discretization.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/flowSheet.py` & `CADET-Process-0.7.1/CADETProcess/processModel/flowSheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
                 if len(connections.destinations) != 0:
                     flag = False
                     warn("Outlet unit cannot have outgoing stream.")
                 if len(connections.origins) == 0:
                     flag = False
                     warn(f"Unit '{unit.name}' does not have ingoing stream.")
             elif isinstance(unit, Cstr):
-                if unit.flow_rate is None and len(connections.destinations) == 0:
+                if unit.flow_rate is not None and len(connections.destinations) == 0:
                     flag = False
                     warn("Cstr cannot have flow rate without outgoing stream.")
             else:
                 if len(connections.origins) == 0:
                     flag = False
                     warn(f"Unit '{unit.name}' does not have ingoing stream.")
                 if len(connections.destinations) == 0:
@@ -725,17 +725,17 @@
 
         # Solve system of equations
         symbols = (
             *unit_total_flow_symbols,
             *unit_inflow_symbols,
             *unit_outflow_symbols
         )
+        symbols = set(symbols)
 
         solution = sym.solve(unit_total_flow_eq + unit_outflow_eq, symbols)
-
         solution = {str(key): value for key, value in solution.items()}
 
         return solution
 
     def check_flow_rates(self, state=None):
         flow_rates = self.get_flow_rates(state)
         for unit, q in flow_rates.items():
```

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/process.py` & `CADET-Process-0.7.1/CADETProcess/processModel/process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/reaction.py` & `CADET-Process-0.7.1/CADETProcess/processModel/reaction.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/solutionRecorder.py` & `CADET-Process-0.7.1/CADETProcess/processModel/solutionRecorder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/processModel/unitOperation.py` & `CADET-Process-0.7.1/CADETProcess/processModel/unitOperation.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/reference.py` & `CADET-Process-0.7.1/CADETProcess/reference.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/settings.py` & `CADET-Process-0.7.1/CADETProcess/settings.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/simulationResults.py` & `CADET-Process-0.7.1/CADETProcess/simulationResults.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/simulator/__init__.py` & `CADET-Process-0.7.1/CADETProcess/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/simulator/cadetAdapter.py` & `CADET-Process-0.7.1/CADETProcess/simulator/cadetAdapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/simulator/simulator.py` & `CADET-Process-0.7.1/CADETProcess/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/smoothing.py` & `CADET-Process-0.7.1/CADETProcess/smoothing.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/smoothing2.py` & `CADET-Process-0.7.1/CADETProcess/smoothing2.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/solution.py` & `CADET-Process-0.7.1/CADETProcess/solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -765,16 +765,15 @@
             )
 
         solution = slice_solution(
             self,
             components=components,
             use_total_concentration=False,
             use_total_concentration_components=False,
-            start=start,
-            end=end,
+            coordinates={'time': [start, end]}
         )
 
         x = solution.time / 60
 
         if layout is None:
             layout = plotting.Layout()
             layout.x_label = '$time~/~min$'
@@ -1189,16 +1188,15 @@
             )
 
         solution = slice_solution(
             self,
             components=components,
             use_total_concentration=False,
             use_total_concentration_components=False,
-            start=start,
-            end=end,
+            coordinates={'time': [start, end]}
         )
 
         x = solution.time / 60
 
         if layout is None:
             layout = plotting.Layout()
             layout.x_label = '$time~/~min$'
```

### Comparing `CADET-Process-0.7.0/CADETProcess/stationarity.py` & `CADET-Process-0.7.1/CADETProcess/stationarity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/tools/yamamoto.py` & `CADET-Process-0.7.1/CADETProcess/tools/yamamoto.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADETProcess/transform.py` & `CADET-Process-0.7.1/CADETProcess/transform.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/CADET_Process.egg-info/PKG-INFO` & `CADET-Process-0.7.1/CADET_Process.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: CADET-Process
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 Home-page: https://github.com/fau-advanced-separations/CADET-Process
 Author: Johannes Schmölder
 Author-email: j.schmoelder@fz-juelich.de
 Project-URL: Bug Tracker, https://github.com/fau-advanced-separations/CADET-Process/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 # CADET-Process
```

### Comparing `CADET-Process-0.7.0/CADET_Process.egg-info/SOURCES.txt` & `CADET-Process-0.7.1/CADET_Process.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/LICENSE` & `CADET-Process-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/PKG-INFO` & `CADET-Process-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: CADET-Process
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 Home-page: https://github.com/fau-advanced-separations/CADET-Process
 Author: Johannes Schmölder
 Author-email: j.schmoelder@fz-juelich.de
 Project-URL: Bug Tracker, https://github.com/fau-advanced-separations/CADET-Process/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 # CADET-Process
```

### Comparing `CADET-Process-0.7.0/README.md` & `CADET-Process-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/batch_elution/optimization_multi.py` & `CADET-Process-0.7.1/examples/batch_elution/optimization_multi.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/batch_elution/optimization_single.py` & `CADET-Process-0.7.1/examples/batch_elution/optimization_single.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/batch_elution/process.py` & `CADET-Process-0.7.1/examples/batch_elution/process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/characterize_chromatographic_system/column_transport_parameters.py` & `CADET-Process-0.7.1/examples/characterize_chromatographic_system/column_transport_parameters.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/characterize_chromatographic_system/particle_porosity.py` & `CADET-Process-0.7.1/examples/characterize_chromatographic_system/particle_porosity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/load_wash_elute/lwe_concentration.py` & `CADET-Process-0.7.1/examples/load_wash_elute/lwe_concentration.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/load_wash_elute/lwe_flow_rate.py` & `CADET-Process-0.7.1/examples/load_wash_elute/lwe_flow_rate.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/recycling/clr_process.py` & `CADET-Process-0.7.1/examples/recycling/clr_process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/examples/recycling/mrssr_process.py` & `CADET-Process-0.7.1/examples/recycling/mrssr_process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/setup.cfg` & `CADET-Process-0.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CADET-Process
-version = 0.7.0
+version = 0.7.1
 author = Johannes Schmölder
 author_email = j.schmoelder@fz-juelich.de
 description = A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fau-advanced-separations/CADET-Process
 project_urls = 
@@ -12,21 +12,21 @@
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 
 [options]
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	numpy>=1.21
 	scipy>=1.7
 	matplotlib>=3.4
 	corner>=2.2.1
-	sympy>=1.8
+	sympy>=1.8,<1.12
 	pathos>=0.2.8
 	addict>=2.4
 	cadet-python>=0.12
 	hopsy>=1.0.0
 	pymoo>=0.6
 	numba>=0.55.1
 	diskcache>=5.4.0
```

### Comparing `CADET-Process-0.7.0/tests/test_binding.py` & `CADET-Process-0.7.1/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_buffer_capacity.py` & `CADET-Process-0.7.1/tests/test_buffer_capacity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_cache.py` & `CADET-Process-0.7.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_carousel.py` & `CADET-Process-0.7.1/tests/test_carousel.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_compartment.py` & `CADET-Process-0.7.1/tests/test_compartment.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_components.py` & `CADET-Process-0.7.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_difference.py` & `CADET-Process-0.7.1/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_equilibrium.py` & `CADET-Process-0.7.1/tests/test_equilibrium.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_events.py` & `CADET-Process-0.7.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_flow_sheet.py` & `CADET-Process-0.7.1/tests/test_flow_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,71 +6,96 @@
 from CADETProcess.processModel import ComponentSystem
 from CADETProcess.processModel import (
     Inlet, Cstr, LumpedRateModelWithoutPores, Outlet
 )
 from CADETProcess.processModel import FlowSheet
 
 
-class Test_flow_sheet(unittest.TestCase):
+def setup_single_cstr_flow_sheet(component_system=None):
+    if component_system is None:
+        component_system = ComponentSystem(2)
 
-    def __init__(self, methodName='runTest'):
-        super().__init__(methodName)
+    cstr = Cstr(component_system, 'cstr')
 
-    def setUp(self):
-        # Batch
-        self.component_system = ComponentSystem(2)
+    flow_sheet = FlowSheet(component_system)
+    flow_sheet.add_unit(cstr)
 
-        flow_sheet = FlowSheet(self.component_system)
+    return flow_sheet
 
-        feed = Inlet(self.component_system, name='feed')
-        eluent = Inlet(self.component_system, name='eluent')
-        column = LumpedRateModelWithoutPores(
-            self.component_system, name='column'
-        )
-        outlet = Outlet(self.component_system, name='outlet')
 
-        flow_sheet.add_unit(feed)
-        flow_sheet.add_unit(eluent)
-        flow_sheet.add_unit(column)
-        flow_sheet.add_unit(outlet)
+def setup_batch_elution_flow_sheet(component_system=None):
+    if component_system is None:
+        component_system = ComponentSystem(2)
 
-        flow_sheet.add_connection(feed, column)
-        flow_sheet.add_connection(eluent, column)
-        flow_sheet.add_connection(column, outlet)
+    flow_sheet = FlowSheet(component_system)
 
-        self.batch_flow_sheet = flow_sheet
+    feed = Inlet(component_system, name='feed')
+    eluent = Inlet(component_system, name='eluent')
+    column = LumpedRateModelWithoutPores(component_system, name='column')
+    outlet = Outlet(component_system, name='outlet')
 
-        # SSR
-        flow_sheet = FlowSheet(self.component_system)
+    flow_sheet.add_unit(feed)
+    flow_sheet.add_unit(eluent)
+    flow_sheet.add_unit(column)
+    flow_sheet.add_unit(outlet)
 
-        feed = Inlet(self.component_system, name='feed')
-        eluent = Inlet(self.component_system, name='eluent')
-        cstr = Cstr(self.component_system, name='cstr')
-        column = LumpedRateModelWithoutPores(
-            self.component_system, name='column'
-        )
-        outlet = Outlet(self.component_system, name='outlet')
+    flow_sheet.add_connection(feed, column)
+    flow_sheet.add_connection(eluent, column)
+    flow_sheet.add_connection(column, outlet)
 
-        flow_sheet.add_unit(feed)
-        flow_sheet.add_unit(eluent)
-        flow_sheet.add_unit(cstr)
-        flow_sheet.add_unit(column)
-        flow_sheet.add_unit(outlet)
+    return flow_sheet
 
-        flow_sheet.add_connection(feed, cstr)
-        flow_sheet.add_connection(cstr, column)
-        flow_sheet.add_connection(eluent, column)
-        flow_sheet.add_connection(column, cstr)
-        flow_sheet.add_connection(column, outlet)
 
-        flow_sheet.add_eluent_inlet(eluent)
-        flow_sheet.add_feed_inlet(feed)
-        flow_sheet.add_product_outlet(outlet)
+def setup_ssr_flow_sheet(component_system=None):
+    if component_system is None:
+        component_system = ComponentSystem(2)
+
+    flow_sheet = FlowSheet(component_system)
+
+    feed = Inlet(component_system, name='feed')
+    eluent = Inlet(component_system, name='eluent')
+    cstr = Cstr(component_system, name='cstr')
+    column = LumpedRateModelWithoutPores(component_system, name='column')
+    outlet = Outlet(component_system, name='outlet')
+
+    flow_sheet.add_unit(feed)
+    flow_sheet.add_unit(eluent)
+    flow_sheet.add_unit(cstr)
+    flow_sheet.add_unit(column)
+    flow_sheet.add_unit(outlet)
+
+    flow_sheet.add_connection(feed, cstr)
+    flow_sheet.add_connection(cstr, column)
+    flow_sheet.add_connection(eluent, column)
+    flow_sheet.add_connection(column, cstr)
+    flow_sheet.add_connection(column, outlet)
+
+    flow_sheet.add_eluent_inlet(eluent)
+    flow_sheet.add_feed_inlet(feed)
+    flow_sheet.add_product_outlet(outlet)
+
+    return flow_sheet
+
 
-        self.ssr_flow_sheet = flow_sheet
+class Test_flow_sheet(unittest.TestCase):
+
+    def __init__(self, methodName='runTest'):
+        super().__init__(methodName)
+
+    def setUp(self):
+        self.component_system = ComponentSystem(2)
+
+        # Single Cstr
+        self.single_cstr_flow_sheet = setup_single_cstr_flow_sheet(self.component_system)
+
+        # Batch
+        self.batch_flow_sheet = setup_batch_elution_flow_sheet(self.component_system)
+
+        # SSR
+        self.ssr_flow_sheet = setup_ssr_flow_sheet(self.component_system)
 
     def test_unit_names(self):
         unit_names_expected = ['feed', 'eluent', 'cstr', 'column', 'outlet']
 
         unit_names = list(self.ssr_flow_sheet.units_dict.keys())
 
         self.assertEqual(self.ssr_flow_sheet.unit_names, unit_names_expected)
@@ -403,21 +428,24 @@
         }
 
         np.testing.assert_equal(
             self.ssr_flow_sheet.get_flow_rates(), expected_flow_rates
         )
 
     def test_check_connectivity(self):
+        self.assertTrue(self.single_cstr_flow_sheet.check_connections())
         self.assertTrue(self.batch_flow_sheet.check_connections())
+        self.assertTrue(self.ssr_flow_sheet.check_connections())
 
         self.batch_flow_sheet.remove_unit('outlet')
 
         with self.assertWarns(Warning):
             self.batch_flow_sheet.check_connections()
 
+
     def test_output_state(self):
         column = self.ssr_flow_sheet.column
 
         output_state_expected = [1, 0]
         output_state = self.ssr_flow_sheet.output_states[column]
         np.testing.assert_equal(output_state, output_state_expected)
```

### Comparing `CADET-Process-0.7.0/tests/test_fractions.py` & `CADET-Process-0.7.1/tests/test_fractions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_individual.py` & `CADET-Process-0.7.1/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_optimization_integration.py` & `CADET-Process-0.7.1/tests/test_optimization_integration.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_optimization_problem.py` & `CADET-Process-0.7.1/tests/test_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_optimization_results.py` & `CADET-Process-0.7.1/tests/test_optimization_results.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_parameters.py` & `CADET-Process-0.7.1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_population.py` & `CADET-Process-0.7.1/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_reaction.py` & `CADET-Process-0.7.1/tests/test_reaction.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_sections.py` & `CADET-Process-0.7.1/tests/test_sections.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_solution.py` & `CADET-Process-0.7.1/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_transform.py` & `CADET-Process-0.7.1/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.0/tests/test_unit_operation.py` & `CADET-Process-0.7.1/tests/test_unit_operation.py`

 * *Files identical despite different names*

