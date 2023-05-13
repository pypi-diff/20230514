# Comparing `tmp/validmind-1.9.3.tar.gz` & `tmp/validmind-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validmind-1.9.3.tar", max compression
+gzip compressed data, was "validmind-1.9.4.tar", max compression
```

## Comparing `validmind-1.9.3.tar` & `validmind-1.9.4.tar`

### file list

```diff
@@ -1,62 +1,64 @@
--rw-r--r--   0        0        0     1295 2023-05-13 15:54:34.670003 validmind-1.9.3/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-05-13 15:54:34.670003 validmind-1.9.3/validmind/__init__.py
--rw-r--r--   0        0        0    11353 2023-05-13 15:54:34.670003 validmind-1.9.3/validmind/api_client.py
--rw-r--r--   0        0        0     9190 2023-05-13 15:54:34.670003 validmind-1.9.3/validmind/client.py
--rw-r--r--   0        0        0      590 2023-05-13 15:54:34.670003 validmind-1.9.3/validmind/data_validation/__init__.py
--rw-r--r--   0        0        0    41101 2023-05-13 15:54:34.674003 validmind-1.9.3/validmind/data_validation/metrics.py
--rw-r--r--   0        0        0    24265 2023-05-13 15:54:34.674003 validmind-1.9.3/validmind/data_validation/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-13 15:54:34.674003 validmind-1.9.3/validmind/datasets/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-13 15:54:34.674003 validmind-1.9.3/validmind/datasets/classification/__init__.py
--rw-r--r--   0        0        0     1330 2023-05-13 15:54:34.674003 validmind-1.9.3/validmind/datasets/classification/customer_churn.py
--rw-r--r--   0        0        0   545707 2023-05-13 15:54:34.674003 validmind-1.9.3/validmind/datasets/classification/datasets/bank_customer_churn.csv
--rw-r--r--   0        0        0  2897191 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/classification/datasets/taiwan_credit.csv
--rw-r--r--   0        0        0     1280 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/classification/taiwan_credit.py
--rw-r--r--   0        0        0     1416 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/__init__.py
--rw-r--r--   0        0        0   107835 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates.csv
--rw-r--r--   0        0        0     2634 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
--rw-r--r--   0        0        0     2634 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
--rw-r--r--   0        0        0     2736 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
--rw-r--r--   0        0        0     3355 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
--rw-r--r--   0        0        0     3866 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
--rw-r--r--   0        0        0    11624 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
--rw-r--r--   0        0        0     4378 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/fred.py
--rw-r--r--   0        0        0     2346 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/lending_club.py
--rw-r--r--   0        0        0    40067 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
--rw-r--r--   0        0        0    48314 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
--rw-r--r--   0        0        0    40063 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
--rw-r--r--   0        0        0    48292 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
--rw-r--r--   0        0        0    60343 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
--rw-r--r--   0        0        0    10529 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_utils.py
--rw-r--r--   0        0        0     1290 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/__init__.py
--rw-r--r--   0        0        0     6712 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/sklearn/__init__.py
--rw-r--r--   0        0        0    13048 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/sklearn/metrics.py
--rw-r--r--   0        0        0    31402 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/sklearn/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/statsmodels/__init__.py
--rw-r--r--   0        0        0    28873 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/statsmodels/metrics.py
--rw-r--r--   0        0        0     1317 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/statsmodels/threshold_tests.py
--rw-r--r--   0        0        0     1657 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/model_validation/utils.py
--rw-r--r--   0        0        0     4788 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/test_plans/__init__.py
--rw-r--r--   0        0        0     2016 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/test_plans/binary_classifier.py
--rw-r--r--   0        0        0      811 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/test_plans/statsmodels_timeseries.py
--rw-r--r--   0        0        0     1604 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/test_plans/tabular_datasets.py
--rw-r--r--   0        0        0     3711 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/test_plans/time_series.py
--rw-r--r--   0        0        0     1988 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/test_suites/__init__.py
--rw-r--r--   0        0        0     1750 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/test_suites/test_suites.py
--rw-r--r--   0        0        0     6465 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/utils.py
--rw-r--r--   0        0        0     1116 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/__init__.py
--rw-r--r--   0        0        0    10713 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/dataset.py
--rw-r--r--   0        0        0     8287 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/dataset_utils.py
--rw-r--r--   0        0        0      592 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/figure.py
--rw-r--r--   0        0        0     3746 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/metric.py
--rw-r--r--   0        0        0     1757 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/metric_result.py
--rw-r--r--   0        0        0     6530 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/model.py
--rw-r--r--   0        0        0     3721 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/plot_utils.py
--rw-r--r--   0        0        0     1518 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/result_summary.py
--rw-r--r--   0        0        0     2501 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/test_context.py
--rw-r--r--   0        0        0    11803 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/test_plan.py
--rw-r--r--   0        0        0    18529 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/test_plan_result.py
--rw-r--r--   0        0        0     1698 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/test_result.py
--rw-r--r--   0        0        0     5019 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/test_suite.py
--rw-r--r--   0        0        0     3620 2023-05-13 15:54:34.694003 validmind-1.9.3/validmind/vm_models/threshold_test.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0     3695 2023-05-13 23:49:55.578990 validmind-1.9.4/LICENSE
+-rw-r--r--   0        0        0     1295 2023-05-13 23:49:55.975006 validmind-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1443 2023-05-13 23:49:55.975006 validmind-1.9.4/validmind/__init__.py
+-rw-r--r--   0        0        0    11353 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/api_client.py
+-rw-r--r--   0        0        0     9190 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/client.py
+-rw-r--r--   0        0        0      590 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/data_validation/__init__.py
+-rw-r--r--   0        0        0    41145 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/data_validation/metrics.py
+-rw-r--r--   0        0        0    24265 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/data_validation/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/datasets/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/datasets/classification/__init__.py
+-rw-r--r--   0        0        0     1330 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/datasets/classification/customer_churn.py
+-rw-r--r--   0        0        0   545707 2023-05-13 23:49:55.983006 validmind-1.9.4/validmind/datasets/classification/datasets/bank_customer_churn.csv
+-rw-r--r--   0        0        0  2897191 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/classification/datasets/taiwan_credit.csv
+-rw-r--r--   0        0        0     1280 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/classification/taiwan_credit.py
+-rw-r--r--   0        0        0     1416 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/__init__.py
+-rw-r--r--   0        0        0   107835 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates.csv
+-rw-r--r--   0        0        0     2634 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
+-rw-r--r--   0        0        0     2634 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
+-rw-r--r--   0        0        0     2736 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
+-rw-r--r--   0        0        0     3355 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
+-rw-r--r--   0        0        0     3866 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
+-rw-r--r--   0        0        0    11624 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
+-rw-r--r--   0        0        0     4378 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/fred.py
+-rw-r--r--   0        0        0     2346 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/lending_club.py
+-rw-r--r--   0        0        0    40067 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
+-rw-r--r--   0        0        0    48314 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
+-rw-r--r--   0        0        0    40063 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
+-rw-r--r--   0        0        0    48292 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
+-rw-r--r--   0        0        0    60343 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
+-rw-r--r--   0        0        0    10529 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_utils.py
+-rw-r--r--   0        0        0     1290 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/__init__.py
+-rw-r--r--   0        0        0     6712 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/sklearn/__init__.py
+-rw-r--r--   0        0        0    13050 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/sklearn/metrics.py
+-rw-r--r--   0        0        0    31402 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/sklearn/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/statsmodels/__init__.py
+-rw-r--r--   0        0        0    29618 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/statsmodels/metrics.py
+-rw-r--r--   0        0        0     1317 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/statsmodels/threshold_tests.py
+-rw-r--r--   0        0        0     1657 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/utils.py
+-rw-r--r--   0        0        0      291 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/statsutils.py
+-rw-r--r--   0        0        0     4788 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/__init__.py
+-rw-r--r--   0        0        0     2016 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/binary_classifier.py
+-rw-r--r--   0        0        0      811 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/statsmodels_timeseries.py
+-rw-r--r--   0        0        0     1604 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/tabular_datasets.py
+-rw-r--r--   0        0        0     3711 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/time_series.py
+-rw-r--r--   0        0        0     1988 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_suites/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_suites/test_suites.py
+-rw-r--r--   0        0        0     6465 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/utils.py
+-rw-r--r--   0        0        0     1116 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/__init__.py
+-rw-r--r--   0        0        0    11061 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/dataset.py
+-rw-r--r--   0        0        0     8287 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/dataset_utils.py
+-rw-r--r--   0        0        0      592 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/figure.py
+-rw-r--r--   0        0        0     3746 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/metric.py
+-rw-r--r--   0        0        0     1757 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/metric_result.py
+-rw-r--r--   0        0        0     6530 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/model.py
+-rw-r--r--   0        0        0     3721 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/plot_utils.py
+-rw-r--r--   0        0        0     1518 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/result_summary.py
+-rw-r--r--   0        0        0     2501 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_context.py
+-rw-r--r--   0        0        0    11803 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_plan.py
+-rw-r--r--   0        0        0    18529 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_plan_result.py
+-rw-r--r--   0        0        0     1698 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_result.py
+-rw-r--r--   0        0        0     5019 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_suite.py
+-rw-r--r--   0        0        0     3620 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/threshold_test.py
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.4/PKG-INFO
```

### Comparing `validmind-1.9.3/pyproject.toml` & `validmind-1.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # include = [
 #   "validmind/**/*.c",
 #   "validmind/**/*.pyx",
 #   "validmind/**/*.pyd",
 #   "validmind/**/*.so",
 # ]
 name = "validmind"
-version = "1.9.3"
+version = "1.9.4"
 
 [tool.poetry.dependencies]
 arch = "^5.4.0"
 click = "^8.0.4"
 dython = "^0.7.1"
 ipython = "^8.11.0"
 myst-parser = "^1.0.0"
```

### Comparing `validmind-1.9.3/validmind/__init__.py` & `validmind-1.9.4/validmind/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/api_client.py` & `validmind-1.9.4/validmind/api_client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/client.py` & `validmind-1.9.4/validmind/client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/data_validation/__init__.py` & `validmind-1.9.4/validmind/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/data_validation/metrics.py` & `validmind-1.9.4/validmind/data_validation/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
 class ScatterPlot(Metric):
     """
     Generates a visual analysis of data by plotting a scatter plot matrix for all columns
     in the dataset. The input dataset can have multiple columns (features) if necessary.
     """
 
     name = "scatter_plot"
-    required_context = ["dataset"]
+    required_context = ["dataset", "dataset.target_column"]
     default_params = {"columns": None}
 
     def run(self):
         if "columns" not in self.params:
             raise ValueError("Columns must be provided in params")
 
         # If no columns are specified in the config, we plot all columns
@@ -462,17 +462,16 @@
         )
         plt.xlabel("Lags")
         plt.ylabel("Independent Variables")
 
         return plt.gcf()
 
     def run(self):
-        target_col = [self.dataset.y.name]
-        independent_vars = list(self.dataset.x.columns)
-
+        target_col = [self.dataset.target_column]
+        independent_vars = list(self.dataset.get_features_columns())
         num_lags = self.params.get("num_lags", 10)
 
         if isinstance(target_col, list) and len(target_col) == 1:
             target_col = target_col[0]
 
         if not isinstance(target_col, str):
             raise ValueError(
```

### Comparing `validmind-1.9.3/validmind/data_validation/threshold_tests.py` & `validmind-1.9.4/validmind/data_validation/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/classification/__init__.py` & `validmind-1.9.4/validmind/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/classification/customer_churn.py` & `validmind-1.9.4/validmind/datasets/classification/customer_churn.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/classification/datasets/bank_customer_churn.csv` & `validmind-1.9.4/validmind/datasets/classification/datasets/bank_customer_churn.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/classification/datasets/taiwan_credit.csv` & `validmind-1.9.4/validmind/datasets/classification/datasets/taiwan_credit.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/classification/taiwan_credit.py` & `validmind-1.9.4/validmind/datasets/classification/taiwan_credit.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/__init__.py` & `validmind-1.9.4/validmind/datasets/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates.csv` & `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv` & `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv` & `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv` & `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv` & `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv` & `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/datasets/lending_club_loan_rates.csv` & `validmind-1.9.4/validmind/datasets/regression/datasets/lending_club_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/fred.py` & `validmind-1.9.4/validmind/datasets/regression/fred.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/lending_club.py` & `validmind-1.9.4/validmind/datasets/regression/lending_club.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl` & `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl` & `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl` & `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl` & `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl` & `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/model_utils.py` & `validmind-1.9.4/validmind/model_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/model_validation/__init__.py` & `validmind-1.9.4/validmind/model_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/model_validation/model_metadata.py` & `validmind-1.9.4/validmind/model_validation/model_metadata.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/model_validation/sklearn/metrics.py` & `validmind-1.9.4/validmind/model_validation/sklearn/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
         :params type: mean, summary
         :params shap_values: a matrix
         :params x_test:
         """
         plt.close("all")
 
         # preserve styles
-        mpl.rcParams["grid.color"] = "#CCC"
+        # mpl.rcParams["grid.color"] = "#CCC"
         ax = plt.axes()
         ax.set_facecolor("white")
 
         summary_plot_extra_args = {}
         if type_ == "mean":
             summary_plot_extra_args = {"plot_type": "bar"}
```

### Comparing `validmind-1.9.3/validmind/model_validation/sklearn/threshold_tests.py` & `validmind-1.9.4/validmind/model_validation/sklearn/threshold_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -728,15 +728,15 @@
                     temp_train_df[feature].to_list(), x_std_dev
                 )
                 temp_test_df[feature] = self.add_noise_std_dev(
                     temp_test_df[feature].to_list(), x_std_dev
                 )
 
             self._compute_metrics(
-                results, temp_train_df, train_y_true, x_std_dev, "Traning"
+                results, temp_train_df, train_y_true, x_std_dev, "Training"
             )
             self._compute_metrics(results, temp_test_df, test_y_true, x_std_dev, "Test")
 
         fig, df = self._plot_robustness(results, features_list)
 
         test_figures.append(
             Figure(
@@ -847,15 +847,15 @@
             palette=["red", "blue"],
             ax=ax,
         )
         ax.tick_params(axis="x")
         ax.set_ylabel("Accuracy", weight="bold", fontsize=22)
         ax.legend(fontsize=22)
         ax.set_xlabel(
-            "Perturbation Size ( X * Standard Deviation)", weight="bold", fontsize=22
+            "Perturbation Size (X * Standard Deviation)", weight="bold", fontsize=22
         )
         ax.set_title(
             f"Perturbed Features: {', '.join(features_columns)}",
             weight="bold",
             fontsize=24,
         )
```

### Comparing `validmind-1.9.3/validmind/model_validation/statsmodels/metrics.py` & `validmind-1.9.4/validmind/model_validation/statsmodels/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 from dataclasses import dataclass
 import pandas as pd
 import numpy as np
 from scipy import stats
 import matplotlib.pyplot as plt
 import seaborn as sns
+from sklearn.metrics import r2_score, mean_squared_error
 from statsmodels.tsa.stattools import adfuller
 from statsmodels.tsa.arima.model import ARIMA
 from statsmodels.tsa.stattools import kpss
 from statsmodels.tsa.seasonal import seasonal_decompose
 from statsmodels.stats.stattools import durbin_watson
 from statsmodels.stats.diagnostic import acorr_ljungbox
 from statsmodels.sandbox.stats.runs import runstest_1samp
@@ -21,18 +22,20 @@
 from statsmodels.graphics.tsaplots import plot_acf
 from arch.unitroot import PhillipsPerron
 from arch.unitroot import ZivotAndrews
 from arch.unitroot import DFGLS
 from ...vm_models import (
     Figure,
     Metric,
+    Model,
     ResultSummary,
     ResultTable,
     ResultTableMetadata,
 )
+from ...statsutils import adj_r2_score
 
 
 @dataclass
 class ResidualsVisualInspection(Metric):
     """
     Log plots for visual inspection of residuals
     """
@@ -556,46 +559,36 @@
     """
     Test that output the summary of regression models of statsmodel library.
     """
 
     name = "regression_model_summary"
 
     def run(self):
-        # statsmodels library information
-        module_name = self.model.model.__class__.__module__
-        library_name = module_name.split(".")[0]
-        model_name = self.model.model.__class__.__name__
-
-        if library_name != "statsmodels" or model_name != "RegressionResultsWrapper":
-            raise ValueError(
-                "Only RegressionResultsWrapper models of statsmodels library supported"
-            )
-
-        lib_model = self.model.model
-        # List of features columns
-        X_columns = lib_model.model.exog_names
-
-        # Extract R-squared and Adjusted R-squared
-        r2 = lib_model.rsquared
-        adj_r2 = lib_model.rsquared_adj
-
-        # Calculate the Mean Squared Error (MSE) and Root Mean Squared Error (RMSE)
-        mse = lib_model.mse_resid
-        rmse = mse**0.5
-
-        # Create a DataFrame for the results
-        summary_regression = pd.DataFrame(
-            {
-                "Independent Variables": [X_columns],
-                "R-Squared": [r2],
-                "Adjusted R-Squared": [adj_r2],
-                "MSE": [mse],
-                "RMSE": [rmse],
-            }
-        )
+        if not Model.is_supported_model(self.model.model):
+            raise ValueError(f"{Model.model_library(self.model.model)}.{Model.model_class(self.model.model)} \
+                              is not supported by ValidMind framework yet")
+
+        X_columns = self.model.train_ds.get_features_columns()
+
+        y_true = self.model.train_ds.y
+        y_pred = self.model.model.predict(self.model.train_ds.x)
+
+        r2 = r2_score(y_true, y_pred)
+        adj_r2 = adj_r2_score(y_true, y_pred, len(y_true), len(X_columns))
+        mse = mean_squared_error(y_true=y_true, y_pred=y_pred, squared=True)
+        rmse = mean_squared_error(y_true=y_true, y_pred=y_pred, squared=False)
+
+        results = {
+            "Independent Variables": X_columns,
+            "R-Squared": r2,
+            "Adjusted R-Squared": adj_r2,
+            "MSE": mse,
+            "RMSE": rmse,
+        }
+        summary_regression = pd.DataFrame(results)
 
         return self.cache_results(
             {
                 "regression_analysis": summary_regression.to_dict(orient="records"),
             }
         )
 
@@ -639,20 +632,18 @@
         all_models = []
         if self.model is not None:
             all_models.append(self.model)
 
         if self.models is not None:
             all_models.extend(self.models)
 
-        for model in all_models:
-            if model.model.__class__.__name__ != "RegressionResultsWrapper":
-                raise ValueError(
-                    "Only RegressionResultsWrapper models of statsmodels library supported"
-                )
-
+        for m in all_models:
+            if not Model.is_supported_model(m.model):
+                raise ValueError(f"{Model.model_library(m.model)}.{Model.model_class(m.model)} \
+                              is not supported by ValidMind framework yet")
         results = self._in_sample_performance_ols(all_models)
         return self.cache_results(
             {
                 "in_sample_performance": pd.DataFrame(results).to_dict(
                     orient="records"
                 ),
             }
@@ -674,22 +665,23 @@
         - 'Adjusted R-Squared': The adjusted R-squared value of the model.
         - 'MSE': The mean squared error of the model.
         - 'RMSE': The root mean squared error of the model.
         """
         evaluation_results = []
 
         for i, model in enumerate(models):
-            X_columns = model.model.model.exog_names
-            # Extract R-squared and Adjusted R-squared
-            r2 = model.model.rsquared
-            adj_r2 = model.model.rsquared_adj
+            X_columns = model.train_ds.get_features_columns()
+            y_true = self.model.train_ds.y
+            y_pred = self.model.model.predict(self.model.train_ds.x)
 
-            # Calculate the Mean Squared Error (MSE) and Root Mean Squared Error (RMSE)
-            mse = model.model.mse_resid
-            rmse = mse**0.5
+            # Extract R-squared and Adjusted R-squared
+            r2 = r2_score(y_true, y_pred)
+            adj_r2 = adj_r2_score(y_true, y_pred, len(y_true), len(X_columns))
+            mse = mean_squared_error(y_true=y_true, y_pred=y_pred, squared=True)
+            rmse = mean_squared_error(y_true=y_true, y_pred=y_pred, squared=False)
 
             # Append the results to the evaluation_results list
             evaluation_results.append(
                 {
                     "Model": f"Model_{i + 1}",
                     "Independent Variables": X_columns,
                     "R-Squared": r2,
@@ -743,18 +735,17 @@
         if self.model is not None:
             all_models.append(self.model)
 
         if self.models is not None:
             all_models.extend(self.models)
 
         for model in all_models:
-            if model.model.__class__.__name__ != "RegressionResultsWrapper":
-                raise ValueError(
-                    "Only RegressionResultsWrapper models of statsmodels library supported"
-                )
+            if not Model.is_supported_model(model.model):
+                raise ValueError(f"{Model.model_library(model.model)}.{Model.model_class(model.model)} \
+                                is not supported by ValidMind framework yet")
             if model.test_ds is None:
                 raise ValueError(
                     "Test dataset is missing in the ValidMind Model object"
                 )
 
         results = self._out_sample_performance_ols(
             all_models,
@@ -780,15 +771,15 @@
         """
 
         # Initialize a list to store results
         results = []
 
         for fitted_model in model_list:
             # Extract the column names of the independent variables from the model
-            independent_vars = fitted_model.model.model.exog_names
+            independent_vars = fitted_model.train_ds.get_features_columns()
 
             # Separate the target variable and features in the test dataset
             X_test = fitted_model.test_ds.x
             y_test = fitted_model.test_ds.y
 
             # Predict the test data
             y_pred = fitted_model.model.predict(X_test)
@@ -852,46 +843,61 @@
         end_date = self.params["end_date"]
 
         # Check models list is not empty
         if not self.models:
             raise ValueError("List of models must be provided in the models parameter")
         all_models = []
         for model in self.models:
-            if model.model.__class__.__name__ != "RegressionResultsWrapper":
-                raise ValueError(
-                    "Only RegressionResultsWrapper models of statsmodels library supported"
-                )
+            if not Model.is_supported_model(model.model):
+                raise ValueError(f"{Model.model_library(model.model)}.{Model.model_class(model.model)} \
+                                 is not supported by ValidMind framework yet")
             all_models.append(model)
 
         figures = self._plot_forecast(all_models, start_date, end_date)
 
         return self.cache_results(figures=figures)
 
     def _plot_forecast(self, model_list, start_date=None, end_date=None):
+        # Convert start_date and end_date to pandas Timestamp for comparison
+        start_date = pd.Timestamp(start_date)
+        end_date = pd.Timestamp(end_date)
+
         # Initialize a list to store figures
         figures = []
 
         for fitted_model in model_list:
             train_ds = fitted_model.train_ds
             test_ds = fitted_model.test_ds
-
+            y_pred = fitted_model.model.predict(fitted_model.train_ds.x)
+            y_pred_test = fitted_model.model.predict(fitted_model.test_ds.x)
             # Check that start_date and end_date are within the data range
             all_dates = pd.concat([pd.Series(train_ds.index), pd.Series(test_ds.index)])
 
             # If start_date or end_date are None, set them to the min/max of all_dates
             if start_date is None:
                 start_date = all_dates.min()
             else:
                 start_date = pd.Timestamp(start_date)
 
             if end_date is None:
                 end_date = all_dates.max()
             else:
                 end_date = pd.Timestamp(end_date)
 
+            # If start_date or end_date are None, set them to the min/max of all_dates
+            if start_date is None:
+                start_date = all_dates.min()
+            else:
+                start_date = pd.Timestamp(start_date)
+
+            if end_date is None:
+                end_date = all_dates.max()
+            else:
+                end_date = pd.Timestamp(end_date)
+
             if start_date < all_dates.min() or end_date > all_dates.max():
                 raise ValueError(
                     "start_date and end_date must be within the range of dates in the data"
                 )
 
             fig, ax = plt.subplots()
             sns.lineplot(
@@ -904,31 +910,31 @@
                 x=test_ds.index,
                 y=test_ds.y,
                 ax=ax,
                 label="Test Forecast",
             )
             sns.lineplot(
                 x=train_ds.index,
-                y=fitted_model.y_train_predict.loc[train_ds.index],
+                y=y_pred,
                 ax=ax,
                 label="Train Dataset",
                 color="grey",
             )
             sns.lineplot(
                 x=test_ds.index,
-                y=fitted_model.y_test_predict.loc[test_ds.index],
+                y=y_pred_test,
                 ax=ax,
                 label="Test Dataset",
                 color="black",
             )
             plt.title(
                 f"Forecast vs Observed for {fitted_model.model.__class__.__name__}"
             )
 
             # Set the x-axis limits to zoom in/out
-            plt.xlim(start_date, end_date)
+            # plt.xlim(start_date, end_date)
 
             plt.legend()
             figures.append(Figure(key=self.key, figure=fig, metadata={}))
             plt.close("all")
 
         return figures
```

### Comparing `validmind-1.9.3/validmind/model_validation/statsmodels/threshold_tests.py` & `validmind-1.9.4/validmind/model_validation/statsmodels/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/model_validation/utils.py` & `validmind-1.9.4/validmind/model_validation/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/test_plans/__init__.py` & `validmind-1.9.4/validmind/test_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/test_plans/binary_classifier.py` & `validmind-1.9.4/validmind/test_plans/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/test_plans/statsmodels_timeseries.py` & `validmind-1.9.4/validmind/test_plans/statsmodels_timeseries.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/test_plans/tabular_datasets.py` & `validmind-1.9.4/validmind/test_plans/tabular_datasets.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/test_plans/time_series.py` & `validmind-1.9.4/validmind/test_plans/time_series.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/test_suites/__init__.py` & `validmind-1.9.4/validmind/test_suites/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/test_suites/test_suites.py` & `validmind-1.9.4/validmind/test_suites/test_suites.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/utils.py` & `validmind-1.9.4/validmind/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/__init__.py` & `validmind-1.9.4/validmind/vm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/dataset.py` & `validmind-1.9.4/validmind/vm_models/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,29 @@
 
         Returns:
             str: The type of the feature with the given id
         """
         feature = self.get_feature_by_id(feature_id)
         return feature["type"]
 
+    def get_features_columns(self):
+        """
+        Returns list of features columns
+
+        Returns:
+            list: The list of features columns
+        """
+        return [
+            field_dic["id"]
+            for field_dic in self.fields
+            if (
+                field_dic["id"] != self.target_column
+            )
+        ]
+
     def get_numeric_features_columns(self):
         """
         Returns list of numeric features columns
 
         Returns:
             list: The list of numberic features columns
         """
```

### Comparing `validmind-1.9.3/validmind/vm_models/dataset_utils.py` & `validmind-1.9.4/validmind/vm_models/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/figure.py` & `validmind-1.9.4/validmind/vm_models/figure.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/metric.py` & `validmind-1.9.4/validmind/vm_models/metric.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/metric_result.py` & `validmind-1.9.4/validmind/vm_models/metric_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/model.py` & `validmind-1.9.4/validmind/vm_models/model.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/plot_utils.py` & `validmind-1.9.4/validmind/vm_models/plot_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/result_summary.py` & `validmind-1.9.4/validmind/vm_models/result_summary.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/test_context.py` & `validmind-1.9.4/validmind/vm_models/test_context.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/test_plan.py` & `validmind-1.9.4/validmind/vm_models/test_plan.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/test_plan_result.py` & `validmind-1.9.4/validmind/vm_models/test_plan_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/test_result.py` & `validmind-1.9.4/validmind/vm_models/test_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/test_suite.py` & `validmind-1.9.4/validmind/vm_models/test_suite.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/validmind/vm_models/threshold_test.py` & `validmind-1.9.4/validmind/vm_models/threshold_test.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.3/PKG-INFO` & `validmind-1.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validmind
-Version: 1.9.3
+Version: 1.9.4
 Summary: ValidMind Developer Framework
 Author: Andres Rodriguez
 Author-email: andres@validmind.ai
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

