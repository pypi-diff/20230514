# Comparing `tmp/validmind-1.9.6.tar.gz` & `tmp/validmind-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validmind-1.9.6.tar", max compression
+gzip compressed data, was "validmind-1.9.7.tar", max compression
```

## Comparing `validmind-1.9.6.tar` & `validmind-1.9.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     3695 2023-05-14 09:06:11.925820 validmind-1.9.6/LICENSE
--rw-r--r--   0        0        0     1295 2023-05-14 09:06:12.273825 validmind-1.9.6/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/__init__.py
--rw-r--r--   0        0        0    11540 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/api_client.py
--rw-r--r--   0        0        0     9190 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/client.py
--rw-r--r--   0        0        0      590 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/data_validation/__init__.py
--rw-r--r--   0        0        0    41161 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/data_validation/metrics.py
--rw-r--r--   0        0        0    25398 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/data_validation/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/datasets/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/datasets/classification/__init__.py
--rw-r--r--   0        0        0     1330 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/datasets/classification/customer_churn.py
--rw-r--r--   0        0        0   545707 2023-05-14 09:06:12.277825 validmind-1.9.6/validmind/datasets/classification/datasets/bank_customer_churn.csv
--rw-r--r--   0        0        0  2897191 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/classification/datasets/taiwan_credit.csv
--rw-r--r--   0        0        0     1280 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/classification/taiwan_credit.py
--rw-r--r--   0        0        0     1416 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/__init__.py
--rw-r--r--   0        0        0   107835 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates.csv
--rw-r--r--   0        0        0     2634 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
--rw-r--r--   0        0        0     2634 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
--rw-r--r--   0        0        0     2736 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
--rw-r--r--   0        0        0     3355 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
--rw-r--r--   0        0        0     3866 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
--rw-r--r--   0        0        0    11624 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
--rw-r--r--   0        0        0     4378 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/fred.py
--rw-r--r--   0        0        0     2346 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/lending_club.py
--rw-r--r--   0        0        0    40067 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
--rw-r--r--   0        0        0    48314 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
--rw-r--r--   0        0        0    40063 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
--rw-r--r--   0        0        0    48292 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
--rw-r--r--   0        0        0    60343 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
--rw-r--r--   0        0        0    10529 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_utils.py
--rw-r--r--   0        0        0       43 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/__init__.py
--rw-r--r--   0        0        0     6712 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/sklearn/__init__.py
--rw-r--r--   0        0        0    15135 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/sklearn/metrics.py
--rw-r--r--   0        0        0    31402 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/sklearn/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/statsmodels/__init__.py
--rw-r--r--   0        0        0    29762 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/statsmodels/metrics.py
--rw-r--r--   0        0        0     1317 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/statsmodels/threshold_tests.py
--rw-r--r--   0        0        0     1657 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/utils.py
--rw-r--r--   0        0        0      311 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/statsutils.py
--rw-r--r--   0        0        0     4788 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/__init__.py
--rw-r--r--   0        0        0     1978 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/binary_classifier.py
--rw-r--r--   0        0        0      811 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/statsmodels_timeseries.py
--rw-r--r--   0        0        0     1604 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/tabular_datasets.py
--rw-r--r--   0        0        0     3711 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/time_series.py
--rw-r--r--   0        0        0     1988 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_suites/__init__.py
--rw-r--r--   0        0        0     1750 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_suites/test_suites.py
--rw-r--r--   0        0        0     6769 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/utils.py
--rw-r--r--   0        0        0     1116 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/__init__.py
--rw-r--r--   0        0        0    11031 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/dataset.py
--rw-r--r--   0        0        0     8287 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/dataset_utils.py
--rw-r--r--   0        0        0      592 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/figure.py
--rw-r--r--   0        0        0     3746 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/metric.py
--rw-r--r--   0        0        0     1757 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/metric_result.py
--rw-r--r--   0        0        0     6530 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/model.py
--rw-r--r--   0        0        0     3721 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/plot_utils.py
--rw-r--r--   0        0        0     1518 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/result_summary.py
--rw-r--r--   0        0        0     2501 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_context.py
--rw-r--r--   0        0        0    11798 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_plan.py
--rw-r--r--   0        0        0    14163 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_plan_result.py
--rw-r--r--   0        0        0     1698 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_result.py
--rw-r--r--   0        0        0     5369 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_suite.py
--rw-r--r--   0        0        0     4231 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/threshold_test.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.6/PKG-INFO
+-rw-r--r--   0        0        0     3695 2023-05-14 18:29:50.589401 validmind-1.9.7/LICENSE
+-rw-r--r--   0        0        0     1295 2023-05-14 18:29:50.905426 validmind-1.9.7/pyproject.toml
+-rw-r--r--   0        0        0     1443 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/__init__.py
+-rw-r--r--   0        0        0    11540 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/api_client.py
+-rw-r--r--   0        0        0     9190 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/client.py
+-rw-r--r--   0        0        0      590 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/data_validation/__init__.py
+-rw-r--r--   0        0        0    41161 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/data_validation/metrics.py
+-rw-r--r--   0        0        0    25398 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/data_validation/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/datasets/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/datasets/classification/__init__.py
+-rw-r--r--   0        0        0     1330 2023-05-14 18:29:50.905426 validmind-1.9.7/validmind/datasets/classification/customer_churn.py
+-rw-r--r--   0        0        0   545707 2023-05-14 18:29:50.909426 validmind-1.9.7/validmind/datasets/classification/datasets/bank_customer_churn.csv
+-rw-r--r--   0        0        0  2897191 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/classification/datasets/taiwan_credit.csv
+-rw-r--r--   0        0        0     1280 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/classification/taiwan_credit.py
+-rw-r--r--   0        0        0     1416 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/__init__.py
+-rw-r--r--   0        0        0   107835 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates.csv
+-rw-r--r--   0        0        0     2634 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
+-rw-r--r--   0        0        0     2634 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
+-rw-r--r--   0        0        0     2736 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
+-rw-r--r--   0        0        0     3355 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
+-rw-r--r--   0        0        0     3866 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
+-rw-r--r--   0        0        0    11624 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
+-rw-r--r--   0        0        0     4378 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/fred.py
+-rw-r--r--   0        0        0     2346 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/lending_club.py
+-rw-r--r--   0        0        0    40067 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
+-rw-r--r--   0        0        0    48314 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
+-rw-r--r--   0        0        0    40063 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
+-rw-r--r--   0        0        0    48292 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
+-rw-r--r--   0        0        0    60343 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
+-rw-r--r--   0        0        0    10529 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_utils.py
+-rw-r--r--   0        0        0       43 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/__init__.py
+-rw-r--r--   0        0        0     6712 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/sklearn/__init__.py
+-rw-r--r--   0        0        0    15135 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/sklearn/metrics.py
+-rw-r--r--   0        0        0    34554 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/sklearn/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/statsmodels/__init__.py
+-rw-r--r--   0        0        0    29762 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/statsmodels/metrics.py
+-rw-r--r--   0        0        0     1317 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/statsmodels/threshold_tests.py
+-rw-r--r--   0        0        0     1657 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/model_validation/utils.py
+-rw-r--r--   0        0        0      311 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/statsutils.py
+-rw-r--r--   0        0        0     4788 2023-05-14 18:29:50.925427 validmind-1.9.7/validmind/test_plans/__init__.py
+-rw-r--r--   0        0        0     1978 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/test_plans/binary_classifier.py
+-rw-r--r--   0        0        0      811 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/test_plans/statsmodels_timeseries.py
+-rw-r--r--   0        0        0     1604 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/test_plans/tabular_datasets.py
+-rw-r--r--   0        0        0     3711 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/test_plans/time_series.py
+-rw-r--r--   0        0        0     1988 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/test_suites/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/test_suites/test_suites.py
+-rw-r--r--   0        0        0     6769 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/utils.py
+-rw-r--r--   0        0        0     1116 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/__init__.py
+-rw-r--r--   0        0        0    11031 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/dataset.py
+-rw-r--r--   0        0        0     8287 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/dataset_utils.py
+-rw-r--r--   0        0        0      592 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/figure.py
+-rw-r--r--   0        0        0     3746 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/metric.py
+-rw-r--r--   0        0        0     1757 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/metric_result.py
+-rw-r--r--   0        0        0     6530 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/model.py
+-rw-r--r--   0        0        0     3721 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/plot_utils.py
+-rw-r--r--   0        0        0     1518 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/result_summary.py
+-rw-r--r--   0        0        0     2501 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/test_context.py
+-rw-r--r--   0        0        0    11798 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/test_plan.py
+-rw-r--r--   0        0        0    14163 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/test_plan_result.py
+-rw-r--r--   0        0        0     1698 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/test_result.py
+-rw-r--r--   0        0        0     5369 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/test_suite.py
+-rw-r--r--   0        0        0     4231 2023-05-14 18:29:50.929428 validmind-1.9.7/validmind/vm_models/threshold_test.py
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.7/PKG-INFO
```

### Comparing `validmind-1.9.6/LICENSE` & `validmind-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/pyproject.toml` & `validmind-1.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # include = [
 #   "validmind/**/*.c",
 #   "validmind/**/*.pyx",
 #   "validmind/**/*.pyd",
 #   "validmind/**/*.so",
 # ]
 name = "validmind"
-version = "1.9.6"
+version = "1.9.7"
 
 [tool.poetry.dependencies]
 arch = "^5.4.0"
 click = "^8.0.4"
 dython = "^0.7.1"
 ipython = "^8.11.0"
 myst-parser = "^1.0.0"
```

### Comparing `validmind-1.9.6/validmind/__init__.py` & `validmind-1.9.7/validmind/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/api_client.py` & `validmind-1.9.7/validmind/api_client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/client.py` & `validmind-1.9.7/validmind/client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/data_validation/__init__.py` & `validmind-1.9.7/validmind/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/data_validation/metrics.py` & `validmind-1.9.7/validmind/data_validation/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/data_validation/threshold_tests.py` & `validmind-1.9.7/validmind/data_validation/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/classification/__init__.py` & `validmind-1.9.7/validmind/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/classification/customer_churn.py` & `validmind-1.9.7/validmind/datasets/classification/customer_churn.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/classification/datasets/bank_customer_churn.csv` & `validmind-1.9.7/validmind/datasets/classification/datasets/bank_customer_churn.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/classification/datasets/taiwan_credit.csv` & `validmind-1.9.7/validmind/datasets/classification/datasets/taiwan_credit.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/classification/taiwan_credit.py` & `validmind-1.9.7/validmind/datasets/classification/taiwan_credit.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/__init__.py` & `validmind-1.9.7/validmind/datasets/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates.csv` & `validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv` & `validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv` & `validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv` & `validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv` & `validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv` & `validmind-1.9.7/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/datasets/lending_club_loan_rates.csv` & `validmind-1.9.7/validmind/datasets/regression/datasets/lending_club_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/fred.py` & `validmind-1.9.7/validmind/datasets/regression/fred.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/lending_club.py` & `validmind-1.9.7/validmind/datasets/regression/lending_club.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl` & `validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl` & `validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl` & `validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl` & `validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl` & `validmind-1.9.7/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/model_utils.py` & `validmind-1.9.7/validmind/model_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/model_validation/model_metadata.py` & `validmind-1.9.7/validmind/model_validation/model_metadata.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/model_validation/sklearn/metrics.py` & `validmind-1.9.7/validmind/model_validation/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/model_validation/sklearn/threshold_tests.py` & `validmind-1.9.7/validmind/model_validation/sklearn/threshold_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,21 +164,39 @@
 class OverfitDiagnosis(ThresholdTest):
     """
     Test that identify overfit regions with high residuals by histogram slicing techniques.
     """
 
     category = "model_diagnosis"
     name = "overfit_regions"
-    required_context = ["model"]
+    required_context = ["model", "model.train_ds", "model.test_ds"]
 
     default_params = {"features_columns": None, "cut_off_percentage": 4}
     default_metrics = {
         "accuracy": metrics.accuracy_score,
     }
 
+    def description(self):
+        return """
+        Test that identify overfitting regions based on the train-test performance gap,
+        one can divide the feature space into regions and analyze the train-test performance
+        gap for each region. Regions with a large train-test performance gap can be considered as
+        overfitting regions, indicating that the model is overfitting in those regions.
+
+        Once overfitting regions have been identified, one can use various techniques to address the overfitting.
+        For example, one could use regularization techniques such as L1 or L2 regularization, dropout, or early
+        stopping to prevent the model from overfitting. Alternatively, one could use data augmentation techniques
+        to increase the size of the training data and reduce overfitting.
+
+        Overall, analyzing the train-test performance gap can provide valuable insights into the performance of
+        a machine learning model and help identify overfitting regions that need to be addressed to improve
+        the model's generalization performance.
+
+        """
+
     def run(self):
         if "cut_off_percentage" not in self.params:
             raise ValueError("cut_off_percentage must be provided in params")
         cut_off_percentage = self.params["cut_off_percentage"]
 
         if "features_columns" not in self.params:
             raise ValueError("features_columns must be provided in params")
@@ -409,15 +427,15 @@
 class WeakspotsDiagnosis(ThresholdTest):
     """
     Test that identify weak regions with high residuals by histogram slicing techniques.
     """
 
     category = "model_diagnosis"
     name = "weak_spots"
-    required_context = ["model"]
+    required_context = ["model", "model.train_ds", "model.test_ds"]
 
     default_params = {
         "features_columns": None,
         # Some default values that the user should override
         "thresholds": {
             "accuracy": 0.75,
             "precision": 0.5,
@@ -429,14 +447,27 @@
     default_metrics = {
         "accuracy": metrics.accuracy_score,
         "precision": partial(metrics.precision_score, zero_division=0),
         "recall": partial(metrics.recall_score, zero_division=0),
         "f1": partial(metrics.f1_score, zero_division=0),
     }
 
+    def description(self):
+        return """
+        A weak spots test is a type of testing that is performed on a machine learning model
+        to identify areas where the model may not perform well or may be vulnerable to errors.
+        The purpose of this testing is to identify the limitations and weaknesses of the model
+        so that appropriate measures can be taken to improve its performance.
+        The weak spots test typically involves subjecting the model to different types of data
+        that are different from the data used to train the model. For example, the test data may
+        contain outliers, missing data, or noise that was not present in the training data. The model
+        is then evaluated on this test data using appropriate metrics such as accuracy, precision,
+        recall, F1 score, etc.
+        """
+
     def run(self):
         thresholds = self.params["thresholds"]
 
         # Ensure there is a threshold for each metric
         for metric in self.default_metrics.keys():
             if metric not in thresholds:
                 raise ValueError(f"Threshold for metric {metric} is missing")
@@ -657,29 +688,47 @@
 
         return fig, df
 
 
 @dataclass
 class RobustnessDiagnosis(ThresholdTest):
     """
-    Test robustness of model by perturbing the features column values
+    Test robustness of model by perturbing the features column values by adding noise within scale
+    stardard deviation.
     """
 
     category = "model_diagnosis"
     name = "robustness"
-    required_context = ["model"]
+    required_context = ["model", "model.train_ds", "model.test_ds"]
 
     default_params = {
         "features_columns": None,
         "scaling_factor_std_dev_list": [0.01, 0.02],
     }
     default_metrics = {
         "accuracy": metrics.accuracy_score,
     }
 
+    def description(self):
+        return """
+        The robustness of a machine learning model refers to its ability to maintain performance
+        in the face of perturbations or changes to the input data. One way to test the robustness
+        of a model is by perturbing its input features and observing how the model's performance changes.
+
+        To perturb the input features, one can add random noise or modify the values of the features
+        within a certain range. By perturbing the input features, one can simulate different scenarios
+        in which the input data may be corrupted or incomplete, and test whether the model is able to
+        handle such scenarios.
+
+        The performance of the model can be measured in terms of its accuracy, precision, recall,
+        or any other relevant metric, both before and after perturbing the input features. A model
+        that is robust to perturbations should maintain a high level of performance even after the
+        input features have been perturbed.
+        """
+
     def run(self):
         # Validate X std deviation parameter
         if "scaling_factor_std_dev_list" not in self.params:
             raise ValueError("scaling_factor_std_dev_list must be provided in params")
         x_std_dev_list = self.params["scaling_factor_std_dev_list"]
 
         if self.model is None:
```

### Comparing `validmind-1.9.6/validmind/model_validation/statsmodels/metrics.py` & `validmind-1.9.7/validmind/model_validation/statsmodels/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/model_validation/statsmodels/threshold_tests.py` & `validmind-1.9.7/validmind/model_validation/statsmodels/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/model_validation/utils.py` & `validmind-1.9.7/validmind/model_validation/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/test_plans/__init__.py` & `validmind-1.9.7/validmind/test_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/test_plans/binary_classifier.py` & `validmind-1.9.7/validmind/test_plans/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/test_plans/statsmodels_timeseries.py` & `validmind-1.9.7/validmind/test_plans/statsmodels_timeseries.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/test_plans/tabular_datasets.py` & `validmind-1.9.7/validmind/test_plans/tabular_datasets.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/test_plans/time_series.py` & `validmind-1.9.7/validmind/test_plans/time_series.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/test_suites/__init__.py` & `validmind-1.9.7/validmind/test_suites/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/test_suites/test_suites.py` & `validmind-1.9.7/validmind/test_suites/test_suites.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/utils.py` & `validmind-1.9.7/validmind/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/__init__.py` & `validmind-1.9.7/validmind/vm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/dataset.py` & `validmind-1.9.7/validmind/vm_models/dataset.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/dataset_utils.py` & `validmind-1.9.7/validmind/vm_models/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/figure.py` & `validmind-1.9.7/validmind/vm_models/figure.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/metric.py` & `validmind-1.9.7/validmind/vm_models/metric.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/metric_result.py` & `validmind-1.9.7/validmind/vm_models/metric_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/model.py` & `validmind-1.9.7/validmind/vm_models/model.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/plot_utils.py` & `validmind-1.9.7/validmind/vm_models/plot_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/result_summary.py` & `validmind-1.9.7/validmind/vm_models/result_summary.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/test_context.py` & `validmind-1.9.7/validmind/vm_models/test_context.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/test_plan.py` & `validmind-1.9.7/validmind/vm_models/test_plan.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/test_plan_result.py` & `validmind-1.9.7/validmind/vm_models/test_plan_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/test_result.py` & `validmind-1.9.7/validmind/vm_models/test_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/test_suite.py` & `validmind-1.9.7/validmind/vm_models/test_suite.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/validmind/vm_models/threshold_test.py` & `validmind-1.9.7/validmind/vm_models/threshold_test.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.6/PKG-INFO` & `validmind-1.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validmind
-Version: 1.9.6
+Version: 1.9.7
 Summary: ValidMind Developer Framework
 Author: Andres Rodriguez
 Author-email: andres@validmind.ai
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

