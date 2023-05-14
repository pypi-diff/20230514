# Comparing `tmp/validmind-1.9.5.tar.gz` & `tmp/validmind-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validmind-1.9.5.tar", max compression
+gzip compressed data, was "validmind-1.9.6.tar", max compression
```

## Comparing `validmind-1.9.5.tar` & `validmind-1.9.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     3695 2023-05-14 02:11:48.304351 validmind-1.9.5/LICENSE
--rw-r--r--   0        0        0     1295 2023-05-14 02:11:48.652361 validmind-1.9.5/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/__init__.py
--rw-r--r--   0        0        0    11353 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/api_client.py
--rw-r--r--   0        0        0     9190 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/client.py
--rw-r--r--   0        0        0      590 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/data_validation/__init__.py
--rw-r--r--   0        0        0    41161 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/data_validation/metrics.py
--rw-r--r--   0        0        0    24265 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/data_validation/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/datasets/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/datasets/classification/__init__.py
--rw-r--r--   0        0        0     1330 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/datasets/classification/customer_churn.py
--rw-r--r--   0        0        0   545707 2023-05-14 02:11:48.656362 validmind-1.9.5/validmind/datasets/classification/datasets/bank_customer_churn.csv
--rw-r--r--   0        0        0  2897191 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/classification/datasets/taiwan_credit.csv
--rw-r--r--   0        0        0     1280 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/classification/taiwan_credit.py
--rw-r--r--   0        0        0     1416 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/__init__.py
--rw-r--r--   0        0        0   107835 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates.csv
--rw-r--r--   0        0        0     2634 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
--rw-r--r--   0        0        0     2634 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
--rw-r--r--   0        0        0     2736 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
--rw-r--r--   0        0        0     3355 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
--rw-r--r--   0        0        0     3866 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
--rw-r--r--   0        0        0    11624 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
--rw-r--r--   0        0        0     4378 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/fred.py
--rw-r--r--   0        0        0     2346 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/lending_club.py
--rw-r--r--   0        0        0    40067 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
--rw-r--r--   0        0        0    48314 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
--rw-r--r--   0        0        0    40063 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
--rw-r--r--   0        0        0    48292 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
--rw-r--r--   0        0        0    60343 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
--rw-r--r--   0        0        0    10529 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_utils.py
--rw-r--r--   0        0        0       43 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/__init__.py
--rw-r--r--   0        0        0     6712 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/sklearn/__init__.py
--rw-r--r--   0        0        0    15135 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/sklearn/metrics.py
--rw-r--r--   0        0        0    31402 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/sklearn/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/statsmodels/__init__.py
--rw-r--r--   0        0        0    29762 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/statsmodels/metrics.py
--rw-r--r--   0        0        0     1317 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/statsmodels/threshold_tests.py
--rw-r--r--   0        0        0     1657 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/utils.py
--rw-r--r--   0        0        0      311 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/statsutils.py
--rw-r--r--   0        0        0     4788 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/__init__.py
--rw-r--r--   0        0        0     1978 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/binary_classifier.py
--rw-r--r--   0        0        0      811 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/statsmodels_timeseries.py
--rw-r--r--   0        0        0     1604 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/tabular_datasets.py
--rw-r--r--   0        0        0     3711 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/time_series.py
--rw-r--r--   0        0        0     1988 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_suites/__init__.py
--rw-r--r--   0        0        0     1750 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_suites/test_suites.py
--rw-r--r--   0        0        0     6769 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/utils.py
--rw-r--r--   0        0        0     1116 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/vm_models/__init__.py
--rw-r--r--   0        0        0    11031 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/dataset.py
--rw-r--r--   0        0        0     8287 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/dataset_utils.py
--rw-r--r--   0        0        0      592 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/figure.py
--rw-r--r--   0        0        0     3746 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/metric.py
--rw-r--r--   0        0        0     1757 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/metric_result.py
--rw-r--r--   0        0        0     6530 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/model.py
--rw-r--r--   0        0        0     3721 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/plot_utils.py
--rw-r--r--   0        0        0     1518 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/result_summary.py
--rw-r--r--   0        0        0     2501 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_context.py
--rw-r--r--   0        0        0    11803 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_plan.py
--rw-r--r--   0        0        0    18529 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_plan_result.py
--rw-r--r--   0        0        0     1698 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_result.py
--rw-r--r--   0        0        0     5019 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_suite.py
--rw-r--r--   0        0        0     3620 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/threshold_test.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.5/PKG-INFO
+-rw-r--r--   0        0        0     3695 2023-05-14 09:06:11.925820 validmind-1.9.6/LICENSE
+-rw-r--r--   0        0        0     1295 2023-05-14 09:06:12.273825 validmind-1.9.6/pyproject.toml
+-rw-r--r--   0        0        0     1443 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/__init__.py
+-rw-r--r--   0        0        0    11540 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/api_client.py
+-rw-r--r--   0        0        0     9190 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/client.py
+-rw-r--r--   0        0        0      590 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/data_validation/__init__.py
+-rw-r--r--   0        0        0    41161 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/data_validation/metrics.py
+-rw-r--r--   0        0        0    25398 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/data_validation/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/datasets/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/datasets/classification/__init__.py
+-rw-r--r--   0        0        0     1330 2023-05-14 09:06:12.273825 validmind-1.9.6/validmind/datasets/classification/customer_churn.py
+-rw-r--r--   0        0        0   545707 2023-05-14 09:06:12.277825 validmind-1.9.6/validmind/datasets/classification/datasets/bank_customer_churn.csv
+-rw-r--r--   0        0        0  2897191 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/classification/datasets/taiwan_credit.csv
+-rw-r--r--   0        0        0     1280 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/classification/taiwan_credit.py
+-rw-r--r--   0        0        0     1416 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/__init__.py
+-rw-r--r--   0        0        0   107835 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates.csv
+-rw-r--r--   0        0        0     2634 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
+-rw-r--r--   0        0        0     2634 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
+-rw-r--r--   0        0        0     2736 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
+-rw-r--r--   0        0        0     3355 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
+-rw-r--r--   0        0        0     3866 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
+-rw-r--r--   0        0        0    11624 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
+-rw-r--r--   0        0        0     4378 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/fred.py
+-rw-r--r--   0        0        0     2346 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/lending_club.py
+-rw-r--r--   0        0        0    40067 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
+-rw-r--r--   0        0        0    48314 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
+-rw-r--r--   0        0        0    40063 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
+-rw-r--r--   0        0        0    48292 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
+-rw-r--r--   0        0        0    60343 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
+-rw-r--r--   0        0        0    10529 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_utils.py
+-rw-r--r--   0        0        0       43 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/__init__.py
+-rw-r--r--   0        0        0     6712 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/sklearn/__init__.py
+-rw-r--r--   0        0        0    15135 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/sklearn/metrics.py
+-rw-r--r--   0        0        0    31402 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/sklearn/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/statsmodels/__init__.py
+-rw-r--r--   0        0        0    29762 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/statsmodels/metrics.py
+-rw-r--r--   0        0        0     1317 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/statsmodels/threshold_tests.py
+-rw-r--r--   0        0        0     1657 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/model_validation/utils.py
+-rw-r--r--   0        0        0      311 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/statsutils.py
+-rw-r--r--   0        0        0     4788 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/__init__.py
+-rw-r--r--   0        0        0     1978 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/binary_classifier.py
+-rw-r--r--   0        0        0      811 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/statsmodels_timeseries.py
+-rw-r--r--   0        0        0     1604 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/tabular_datasets.py
+-rw-r--r--   0        0        0     3711 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_plans/time_series.py
+-rw-r--r--   0        0        0     1988 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_suites/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/test_suites/test_suites.py
+-rw-r--r--   0        0        0     6769 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/utils.py
+-rw-r--r--   0        0        0     1116 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/__init__.py
+-rw-r--r--   0        0        0    11031 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/dataset.py
+-rw-r--r--   0        0        0     8287 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/dataset_utils.py
+-rw-r--r--   0        0        0      592 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/figure.py
+-rw-r--r--   0        0        0     3746 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/metric.py
+-rw-r--r--   0        0        0     1757 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/metric_result.py
+-rw-r--r--   0        0        0     6530 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/model.py
+-rw-r--r--   0        0        0     3721 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/plot_utils.py
+-rw-r--r--   0        0        0     1518 2023-05-14 09:06:12.293826 validmind-1.9.6/validmind/vm_models/result_summary.py
+-rw-r--r--   0        0        0     2501 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_context.py
+-rw-r--r--   0        0        0    11798 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_plan.py
+-rw-r--r--   0        0        0    14163 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_plan_result.py
+-rw-r--r--   0        0        0     1698 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_result.py
+-rw-r--r--   0        0        0     5369 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/test_suite.py
+-rw-r--r--   0        0        0     4231 2023-05-14 09:06:12.297826 validmind-1.9.6/validmind/vm_models/threshold_test.py
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.6/PKG-INFO
```

### Comparing `validmind-1.9.5/LICENSE` & `validmind-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/pyproject.toml` & `validmind-1.9.6/pyproject.toml`

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
-version = "1.9.5"
+version = "1.9.6"
 
 [tool.poetry.dependencies]
 arch = "^5.4.0"
 click = "^8.0.4"
 dython = "^0.7.1"
 ipython = "^8.11.0"
 myst-parser = "^1.0.0"
```

### Comparing `validmind-1.9.5/validmind/__init__.py` & `validmind-1.9.6/validmind/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/api_client.py` & `validmind-1.9.6/validmind/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,31 @@
 
 import requests
 
 from .utils import NumpyEncoder
 from .utils import get_full_typename, is_matplotlib_typename
 
 API_HOST = os.environ.get("VM_API_HOST", "http://127.0.0.1:5000/api/v1/tracking")
+API_PROJECT = os.environ.get("VM_API_PROJECT")
 VALID_DATASET_TYPES = ["training", "test", "validation"]
 
 vm_api_key = None
 vm_api_secret = None
 
 api_session = requests.Session()
 
 
+def get_api_host():
+    return API_HOST
+
+
+def get_api_project():
+    return API_PROJECT
+
+
 def __ping():
     r = api_session.get(f"{API_HOST}/ping")
 
     # TODO: handle 401
     if r.status_code != 200:
         print("Unsuccessful ping to ValidMind API")
         raise Exception(r.text)
@@ -64,14 +73,15 @@
     Raises:
         ValueError: If the API key and secret are not provided
 
     Returns:
         bool: True if the ping was successful
     """
     global API_HOST
+    global API_PROJECT
 
     ENV_API_KEY = os.environ.get("VM_API_KEY")
     ENV_API_SECRET = os.environ.get("VM_API_SECRET")
 
     vm_api_key = api_key or ENV_API_KEY
     vm_api_secret = api_secret or ENV_API_SECRET
 
@@ -87,14 +97,16 @@
         {
             "X-API-KEY": vm_api_key,
             "X-API-SECRET": vm_api_secret,
             "X-PROJECT-CUID": project,
         }
     )
 
+    API_PROJECT = project
+
     return __ping()
 
 
 def log_dataset(vm_dataset):
     """
     Logs metadata and statistics about a dataset to ValidMind API.
```

### Comparing `validmind-1.9.5/validmind/client.py` & `validmind-1.9.6/validmind/client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/data_validation/__init__.py` & `validmind-1.9.6/validmind/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/data_validation/metrics.py` & `validmind-1.9.6/validmind/data_validation/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/data_validation/threshold_tests.py` & `validmind-1.9.6/validmind/data_validation/threshold_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,74 @@
 """
 Threshold based tests
 """
 
+from typing import List
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
 from dataclasses import dataclass
 from pandas_profiling.config import Settings
 from pandas_profiling.model.typeset import ProfilingTypeSet
 from scipy import stats
 
-
-from ..vm_models import Dataset, TestResult, Figure, ThresholdTest
+from ..vm_models import (
+    Dataset,
+    TestResult,
+    Figure,
+    ThresholdTest,
+    ResultSummary,
+    ResultTable,
+    ResultTableMetadata,
+)
 
 
 @dataclass
 class ClassImbalance(ThresholdTest):
     """
     The class imbalance test measures the disparity between the majority
     class and the minority class in the target column.
     """
 
     category = "data_quality"
     name = "class_imbalance"
     required_context = ["dataset"]
     default_params = {"min_percent_threshold": 0.2}
 
+    def summary(self, results: List[TestResult], all_passed: bool):
+        """
+        The class imbalance test returns a single result like this:
+        [{"values": {"0": 0.798, "1": 0.202}, "column": "Exited", "passed": true}]
+
+        So we build a table with 2 rows, one for each class.
+        """
+
+        results_table = []
+        result = results[0]
+        for class_name, class_percent in result.values.items():
+            results_table.append(
+                {
+                    "Class": f'{class_name} ({"Negative" if class_name == "0" or class_name == 0 else "Positive"})',
+                    "Percentage of Rows (%)": class_percent * 100,
+                }
+            )
+
+        return ResultSummary(
+            results=[
+                ResultTable(
+                    data=results_table,
+                    metadata=ResultTableMetadata(
+                        title=f"Class Imbalance Results for Column {self.dataset.target_column}"
+                    ),
+                )
+            ]
+        )
+
     def run(self):
         # Can only run this test if we have a Dataset object
         if not isinstance(self.dataset, Dataset):
             raise ValueError("ClassImbalance requires a validmind Dataset object")
 
         if self.dataset.target_column is None:
             print("Skipping class_imbalance test because no target column is defined")
```

### Comparing `validmind-1.9.5/validmind/datasets/classification/__init__.py` & `validmind-1.9.6/validmind/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/classification/customer_churn.py` & `validmind-1.9.6/validmind/datasets/classification/customer_churn.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/classification/datasets/bank_customer_churn.csv` & `validmind-1.9.6/validmind/datasets/classification/datasets/bank_customer_churn.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/classification/datasets/taiwan_credit.csv` & `validmind-1.9.6/validmind/datasets/classification/datasets/taiwan_credit.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/classification/taiwan_credit.py` & `validmind-1.9.6/validmind/datasets/classification/taiwan_credit.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/__init__.py` & `validmind-1.9.6/validmind/datasets/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates.csv` & `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv` & `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv` & `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv` & `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv` & `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv` & `validmind-1.9.6/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/datasets/lending_club_loan_rates.csv` & `validmind-1.9.6/validmind/datasets/regression/datasets/lending_club_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/fred.py` & `validmind-1.9.6/validmind/datasets/regression/fred.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/lending_club.py` & `validmind-1.9.6/validmind/datasets/regression/lending_club.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl` & `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl` & `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl` & `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl` & `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl` & `validmind-1.9.6/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/model_utils.py` & `validmind-1.9.6/validmind/model_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/model_validation/model_metadata.py` & `validmind-1.9.6/validmind/model_validation/model_metadata.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/model_validation/sklearn/metrics.py` & `validmind-1.9.6/validmind/model_validation/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/model_validation/sklearn/threshold_tests.py` & `validmind-1.9.6/validmind/model_validation/sklearn/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/model_validation/statsmodels/metrics.py` & `validmind-1.9.6/validmind/model_validation/statsmodels/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/model_validation/statsmodels/threshold_tests.py` & `validmind-1.9.6/validmind/model_validation/statsmodels/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/model_validation/utils.py` & `validmind-1.9.6/validmind/model_validation/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/test_plans/__init__.py` & `validmind-1.9.6/validmind/test_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/test_plans/binary_classifier.py` & `validmind-1.9.6/validmind/test_plans/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/test_plans/statsmodels_timeseries.py` & `validmind-1.9.6/validmind/test_plans/statsmodels_timeseries.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/test_plans/tabular_datasets.py` & `validmind-1.9.6/validmind/test_plans/tabular_datasets.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/test_plans/time_series.py` & `validmind-1.9.6/validmind/test_plans/time_series.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/test_suites/__init__.py` & `validmind-1.9.6/validmind/test_suites/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/test_suites/test_suites.py` & `validmind-1.9.6/validmind/test_suites/test_suites.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/utils.py` & `validmind-1.9.6/validmind/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/__init__.py` & `validmind-1.9.6/validmind/vm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/dataset.py` & `validmind-1.9.6/validmind/vm_models/dataset.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/dataset_utils.py` & `validmind-1.9.6/validmind/vm_models/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/figure.py` & `validmind-1.9.6/validmind/vm_models/figure.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/metric.py` & `validmind-1.9.6/validmind/vm_models/metric.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/metric_result.py` & `validmind-1.9.6/validmind/vm_models/metric_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/model.py` & `validmind-1.9.6/validmind/vm_models/model.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/plot_utils.py` & `validmind-1.9.6/validmind/vm_models/plot_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/result_summary.py` & `validmind-1.9.6/validmind/vm_models/result_summary.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/test_context.py` & `validmind-1.9.6/validmind/vm_models/test_context.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/test_plan.py` & `validmind-1.9.6/validmind/vm_models/test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,17 +229,16 @@
             self.pbar_description.value = (
                 f"Sending result to ValidMind: {result.result_id}..."
             )
 
             try:
                 result.log()
             except Exception as e:
-                self.pbar.set_description(
-                    f"Failed to log result: {result} for test plan result '{str(result)}'"
-                )
+                print(result)
+                self.pbar_description.value = f"Failed to log result: {result} for test plan result '{str(result)}'"
                 print(e)
                 raise e
 
             self.pbar.value += 1
 
     def _results_title(self) -> str:
         """
```

### Comparing `validmind-1.9.5/validmind/vm_models/test_plan_result.py` & `validmind-1.9.6/validmind/vm_models/test_plan_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 TestPlanResult
 """
 # TODO: we are probably going to want to move all this html generation into an html template file
 # and use something like jinja to render it. This is fine for now, but the html is a bit messy
+import json
 import os
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from io import BytesIO
 from typing import List, Optional
 import base64
@@ -26,14 +27,15 @@
 )
 from .dataset import Dataset
 from .figure import Figure
 from .metric_result import MetricResult
 from .model import Model
 from .result_summary import ResultSummary
 from .test_result import TestResults
+from ..utils import NumpyEncoder
 
 
 def update_metadata(content_id: str, text: str) -> None:
     """
     Update the metadata of a content item. By default we don't
     override the existing metadata, but we can override it by
     setting the VM_OVERRIDE_METADATA environment variable to True
@@ -59,24 +61,22 @@
     for fig in figures:
         tmpfile = BytesIO()
         fig.figure.savefig(tmpfile, format="png")
         encoded = base64.b64encode(tmpfile.getvalue()).decode("utf-8")
         plots.append(
             widgets.HTML(
                 value=f"""
-                <img src="data:image/png;base64,{encoded}"/>
+                <img style="width:100%; height: auto;" src="data:image/png;base64,{encoded}"/>
                 """
             )
         )
 
-    num_columns = len(figures) if len(figures) <= 3 else 3
-
     return widgets.GridBox(
         plots,
-        layout=widgets.Layout(grid_template_columns=f"repeat({num_columns}, 1fr)"),
+        layout=widgets.Layout(grid_template_columns="repeat(3, 1fr)"),
     )
 
 
 @dataclass
 class TestPlanResult(ABC):
     """Base Class for test plan results"""
 
@@ -402,156 +402,36 @@
                 f'{self.__class__.__name__}(result_id="{self.result_id}", test_results)'
             )
         else:
             return f'{self.__class__.__name__}(result_id="{self.result_id}", figures)'
 
     def _to_widget(self):
         vbox_children = []
+
+        test_params = json.dumps(self.test_results.params, cls=NumpyEncoder)
+
         vbox_children.append(
             widgets.HTML(
                 value=f"""
-        <div class="metric-result">
-            <div class="metric-result-body">
-                <div class="test-result-header-title">
-                    <span class="test-result-header-title-text">
-                        {" ".join(self.test_results.test_name.split("_")).title()}
-                    </span>
-                    <span class="test-result-header-title-icon">
-                        {"✅" if self.test_results.passed else "❌"}
-                    </span>
-                </div>
-            </div>
-            <div class="metric-result-body">
-                <div class="metric-body-column">
-                    <div class="metric-body-column-title">Test Name</div>
-                    <div class="metric-body-column-value">{self.test_results.test_name}</div>
-                </div>
-                <div class="metric-body-column">
-                    <div class="metric-body-column-title">Category</div>
-                    <div class="metric-body-column-value">{self.test_results.category}</div>
-                </div>
-                <div class="metric-body-column">
-                    <div class="metric-body-column-title">Passed</div>
-                    <div class="metric-body-column-value">{self.test_results.passed}</div>
-                </div>
-                <div class="metric-body-column">
-                    <div class="metric-body-column-title">Params</div>
-                    <div class="metric-body-column-value">{self.test_results.params}</div>
-                </div>
-            </div>
-            <div class="results-objs" style="display: none;">
-                <div class="results-objs-title">Results</div>
-                <div class="results-objs-body">{self.test_results.results}</div>
-            </div>
-            <div class="metric-result-body">
-                <a onclick="toggleTestResults(this)" style="margin-top: 10px; cursor: pointer; color: blue;">
-                    See Result Details
-                </a>
-            </div>
-        </div>
-        """
+                <h2>{" ".join(self.test_results.test_name.split("_")).title()} {"✅" if self.test_results.passed else "❌"}</h2>
+                <h4>Test Parameters</h4>
+                <pre>{test_params}</pre>
+                """
             )
         )
 
+        if self.test_results.summary:
+            tables = self._summary_tables_to_widget(self.test_results.summary)
+            vbox_children.extend(tables)
+
         if self.figures:
             vbox_children.append(widgets.HTML(value="<h3>Plots</h3>"))
             plot_widgets = plot_figures(self.figures)
             vbox_children.append(plot_widgets)
 
-        vbox_children.append(
-            widgets.HTML(
-                value="""
-        <style>
-            .metric-result {
-                background-color: #F5F5F5;
-                border: 1px solid #e0e0e0;
-                border-radius: 4px;
-                padding: 10px;
-                margin: 10px 0;
-            }
-            .metric-result-body {
-                display: flex;
-                flex-direction: column;
-                justify-content: space-between;
-                gap: 10px;
-            }
-            .metric-body-column {
-                display: flex;
-                flex-direction: column;
-                justify-content: space-between;
-                width: 33%;
-            }
-            .metric-body-column-title {
-                font-size: 16px;
-                font-weight: 600;
-            }
-            .metric-value {
-                display: flex;
-                flex-direction: column;
-                justify-content: space-between;
-                margin-top: 15px;
-            }
-            .metric-value-title {
-                font-size: 16px;
-                font-weight: 600;
-            }
-            .metric-value-value {
-                font-size: 14px;
-                font-weight: 500;
-                margin-top: 10px;
-            }
-            .test-result {
-                border: 1px solid #ccc;
-                border-radius: 5px;
-                margin-bottom: 10px;
-            }
-            .test-result-header {
-                display: flex;
-                justify-content: space-between;
-                align-items: center;
-                padding: 10px;
-            }
-            .test-result-header-title {
-                display: flex;
-                align-items: center;
-            }
-            .test-result-header-title-text {
-                text-decoration: underline;
-                font-size: 18px;
-                font-weight: 600;
-            }
-            .test-result-header-title-icon {
-                margin-left: 10px;
-            }
-            .results-objs {
-                padding: 10px;
-            }
-            .results-objs-title {
-                font-weight: bold;
-            }
-            .results-objs-body {
-                margin-top: 5px;
-            }
-        </style>
-        <script>
-            function toggleTestResults(btn) {{
-                const rslts = btn.parentElement.parentElement.querySelector('.results-objs');
-                if (rslts.style.display === 'none') {{
-                    rslts.style.display = 'block';
-                    btn.innerHTML = 'Hide Result Details';
-                }} else {{
-                    rslts.style.display = 'none';
-                    btn.innerHTML = 'See Result Details';
-                }}
-            }}
-        </script>
-        """
-            )
-        )
-
         return widgets.VBox(vbox_children)
 
     def log(self):
         log_test_result(self.test_results)
         if self.figures:
             for fig in self.figures:
                 log_figure(fig.figure, fig.key, fig.metadata)
```

### Comparing `validmind-1.9.5/validmind/vm_models/test_result.py` & `validmind-1.9.6/validmind/vm_models/test_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.5/validmind/vm_models/test_suite.py` & `validmind-1.9.6/validmind/vm_models/test_suite.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import ipywidgets as widgets
 
 from IPython.display import display
 
 from .test_context import TestContext
 from .test_plan import TestPlan
+from ..api_client import get_api_host, get_api_project
 from ..utils import is_notebook
 
 
 @dataclass
 class TestSuite(TestPlan):
     """
     Base class for test suites. Test suites are used to define any
@@ -124,14 +125,18 @@
         if not is_notebook():
             return
 
         if len(self._test_plan_instances) == 0:
             return
 
         title = widgets.HTML(value=self._results_title())
+        ui_host = get_api_host().replace("/api/v1/tracking", "")
+        results_link = widgets.HTML(
+            value=f'<h3>Click <a href="{ui_host}/projects/{get_api_project()}/project-overview">here</a> to view the updated model documentation for this project.</h3>'
+        )
 
         accordion_contents = self._results_summary()
         accordion_widget = widgets.Accordion(children=accordion_contents)
         for i, _ in enumerate(accordion_widget.children):
             accordion_widget.set_title(
                 i,
                 f"Test Plan: {self._test_plan_instances[i].title()} ({self._test_plan_instances[i].name})",
@@ -147,15 +152,15 @@
                 border: 1px solid #ccc;
                 border-radius: 5px;
             }
         </style>
         """
         )
 
-        html = widgets.VBox([title, accordion_widget, style_footer])
+        html = widgets.VBox([title, results_link, accordion_widget, style_footer])
         display(html)
 
     @property
     def results(self):
         """
         Returns the results of the test suite.
         """
```

### Comparing `validmind-1.9.5/validmind/vm_models/threshold_test.py` & `validmind-1.9.6/validmind/vm_models/threshold_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 TODO: Test definitions should be supported in the API too
 """
 
 from dataclasses import dataclass
 from typing import ClassVar, List, Optional
 
 from .figure import Figure
+from .result_summary import ResultSummary, ResultTable
 from .test_context import TestContext, TestContextUtils
 from .test_plan_result import TestPlanTestResult
 from .test_result import TestResult, TestResults
 from ..utils import clean_docstring
 
 
 @dataclass
@@ -51,23 +52,39 @@
     def description(self):
         """
         Return the test description. Should be overridden by subclasses. Defaults
         to returning the class' docstring
         """
         return self.__doc__.strip()
 
-    def summary(self, result: Optional[TestResults] = None):
+    def summary(self, results: Optional[List[TestResult]], all_passed: bool):
         """
-        Return the threshold test summary. Should be overridden by subclasses. Defaults to None.
+        Return the threshold test summary. Should be overridden by subclasses. Defaults to showing
+        a table with test_name(optional), column and passed.
+
         The test summary allows renderers (e.g. Word and ValidMind UI) to display a
         short summary of the test results.
-
-        We return None here because the test summary is optional.
         """
-        return None
+        if results is None:
+            return None
+
+        results_table = []
+        for test_result in results:
+            result_object = {
+                "passed": test_result.passed,
+            }
+
+            if test_result.test_name is not None:
+                result_object["test_name"] = test_result.test_name
+            if test_result.column is not None:
+                result_object["column"] = test_result.column
+
+            results_table.append(result_object)
+
+        return ResultSummary(results=[ResultTable(data=results_table)])
 
     def run(self, *args, **kwargs):
         """
         Run the test and cache its results
         """
         raise NotImplementedError
 
@@ -92,15 +109,15 @@
         result_metadata = [
             {
                 "content_id": f"test_description:{self.name}",
                 "text": clean_docstring(self.description()),
             }
         ]
 
-        result_summary = self.summary(test_results_list)
+        result_summary = self.summary(test_results_list, passed)
 
         self.result = TestPlanTestResult(
             result_id=self.name,
             result_metadata=result_metadata,
             test_results=TestResults(
                 category=self.category,
                 test_name=self.name,
```

### Comparing `validmind-1.9.5/PKG-INFO` & `validmind-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validmind
-Version: 1.9.5
+Version: 1.9.6
 Summary: ValidMind Developer Framework
 Author: Andres Rodriguez
 Author-email: andres@validmind.ai
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

