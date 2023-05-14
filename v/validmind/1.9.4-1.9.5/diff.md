# Comparing `tmp/validmind-1.9.4.tar.gz` & `tmp/validmind-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validmind-1.9.4.tar", max compression
+gzip compressed data, was "validmind-1.9.5.tar", max compression
```

## Comparing `validmind-1.9.4.tar` & `validmind-1.9.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     3695 2023-05-13 23:49:55.578990 validmind-1.9.4/LICENSE
--rw-r--r--   0        0        0     1295 2023-05-13 23:49:55.975006 validmind-1.9.4/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-05-13 23:49:55.975006 validmind-1.9.4/validmind/__init__.py
--rw-r--r--   0        0        0    11353 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/api_client.py
--rw-r--r--   0        0        0     9190 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/client.py
--rw-r--r--   0        0        0      590 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/data_validation/__init__.py
--rw-r--r--   0        0        0    41145 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/data_validation/metrics.py
--rw-r--r--   0        0        0    24265 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/data_validation/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/datasets/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/datasets/classification/__init__.py
--rw-r--r--   0        0        0     1330 2023-05-13 23:49:55.979006 validmind-1.9.4/validmind/datasets/classification/customer_churn.py
--rw-r--r--   0        0        0   545707 2023-05-13 23:49:55.983006 validmind-1.9.4/validmind/datasets/classification/datasets/bank_customer_churn.csv
--rw-r--r--   0        0        0  2897191 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/classification/datasets/taiwan_credit.csv
--rw-r--r--   0        0        0     1280 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/classification/taiwan_credit.py
--rw-r--r--   0        0        0     1416 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/__init__.py
--rw-r--r--   0        0        0   107835 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates.csv
--rw-r--r--   0        0        0     2634 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
--rw-r--r--   0        0        0     2634 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
--rw-r--r--   0        0        0     2736 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
--rw-r--r--   0        0        0     3355 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
--rw-r--r--   0        0        0     3866 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
--rw-r--r--   0        0        0    11624 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
--rw-r--r--   0        0        0     4378 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/fred.py
--rw-r--r--   0        0        0     2346 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/lending_club.py
--rw-r--r--   0        0        0    40067 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
--rw-r--r--   0        0        0    48314 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
--rw-r--r--   0        0        0    40063 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
--rw-r--r--   0        0        0    48292 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
--rw-r--r--   0        0        0    60343 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
--rw-r--r--   0        0        0    10529 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_utils.py
--rw-r--r--   0        0        0     1290 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/__init__.py
--rw-r--r--   0        0        0     6712 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/sklearn/__init__.py
--rw-r--r--   0        0        0    13050 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/sklearn/metrics.py
--rw-r--r--   0        0        0    31402 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/sklearn/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/statsmodels/__init__.py
--rw-r--r--   0        0        0    29618 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/statsmodels/metrics.py
--rw-r--r--   0        0        0     1317 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/statsmodels/threshold_tests.py
--rw-r--r--   0        0        0     1657 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/model_validation/utils.py
--rw-r--r--   0        0        0      291 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/statsutils.py
--rw-r--r--   0        0        0     4788 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/__init__.py
--rw-r--r--   0        0        0     2016 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/binary_classifier.py
--rw-r--r--   0        0        0      811 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/statsmodels_timeseries.py
--rw-r--r--   0        0        0     1604 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/tabular_datasets.py
--rw-r--r--   0        0        0     3711 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_plans/time_series.py
--rw-r--r--   0        0        0     1988 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_suites/__init__.py
--rw-r--r--   0        0        0     1750 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/test_suites/test_suites.py
--rw-r--r--   0        0        0     6465 2023-05-13 23:49:55.999007 validmind-1.9.4/validmind/utils.py
--rw-r--r--   0        0        0     1116 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/__init__.py
--rw-r--r--   0        0        0    11061 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/dataset.py
--rw-r--r--   0        0        0     8287 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/dataset_utils.py
--rw-r--r--   0        0        0      592 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/figure.py
--rw-r--r--   0        0        0     3746 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/metric.py
--rw-r--r--   0        0        0     1757 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/metric_result.py
--rw-r--r--   0        0        0     6530 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/model.py
--rw-r--r--   0        0        0     3721 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/plot_utils.py
--rw-r--r--   0        0        0     1518 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/result_summary.py
--rw-r--r--   0        0        0     2501 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_context.py
--rw-r--r--   0        0        0    11803 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_plan.py
--rw-r--r--   0        0        0    18529 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_plan_result.py
--rw-r--r--   0        0        0     1698 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_result.py
--rw-r--r--   0        0        0     5019 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/test_suite.py
--rw-r--r--   0        0        0     3620 2023-05-13 23:49:56.003007 validmind-1.9.4/validmind/vm_models/threshold_test.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0     3695 2023-05-14 02:11:48.304351 validmind-1.9.5/LICENSE
+-rw-r--r--   0        0        0     1295 2023-05-14 02:11:48.652361 validmind-1.9.5/pyproject.toml
+-rw-r--r--   0        0        0     1443 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/__init__.py
+-rw-r--r--   0        0        0    11353 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/api_client.py
+-rw-r--r--   0        0        0     9190 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/client.py
+-rw-r--r--   0        0        0      590 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/data_validation/__init__.py
+-rw-r--r--   0        0        0    41161 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/data_validation/metrics.py
+-rw-r--r--   0        0        0    24265 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/data_validation/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/datasets/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/datasets/classification/__init__.py
+-rw-r--r--   0        0        0     1330 2023-05-14 02:11:48.652361 validmind-1.9.5/validmind/datasets/classification/customer_churn.py
+-rw-r--r--   0        0        0   545707 2023-05-14 02:11:48.656362 validmind-1.9.5/validmind/datasets/classification/datasets/bank_customer_churn.csv
+-rw-r--r--   0        0        0  2897191 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/classification/datasets/taiwan_credit.csv
+-rw-r--r--   0        0        0     1280 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/classification/taiwan_credit.py
+-rw-r--r--   0        0        0     1416 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/__init__.py
+-rw-r--r--   0        0        0   107835 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates.csv
+-rw-r--r--   0        0        0     2634 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
+-rw-r--r--   0        0        0     2634 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
+-rw-r--r--   0        0        0     2736 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
+-rw-r--r--   0        0        0     3355 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
+-rw-r--r--   0        0        0     3866 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
+-rw-r--r--   0        0        0    11624 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
+-rw-r--r--   0        0        0     4378 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/fred.py
+-rw-r--r--   0        0        0     2346 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/lending_club.py
+-rw-r--r--   0        0        0    40067 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
+-rw-r--r--   0        0        0    48314 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
+-rw-r--r--   0        0        0    40063 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
+-rw-r--r--   0        0        0    48292 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
+-rw-r--r--   0        0        0    60343 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
+-rw-r--r--   0        0        0    10529 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_utils.py
+-rw-r--r--   0        0        0       43 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/__init__.py
+-rw-r--r--   0        0        0     6712 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/sklearn/__init__.py
+-rw-r--r--   0        0        0    15135 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/sklearn/metrics.py
+-rw-r--r--   0        0        0    31402 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/sklearn/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/statsmodels/__init__.py
+-rw-r--r--   0        0        0    29762 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/statsmodels/metrics.py
+-rw-r--r--   0        0        0     1317 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/statsmodels/threshold_tests.py
+-rw-r--r--   0        0        0     1657 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/model_validation/utils.py
+-rw-r--r--   0        0        0      311 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/statsutils.py
+-rw-r--r--   0        0        0     4788 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/__init__.py
+-rw-r--r--   0        0        0     1978 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/binary_classifier.py
+-rw-r--r--   0        0        0      811 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/statsmodels_timeseries.py
+-rw-r--r--   0        0        0     1604 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/tabular_datasets.py
+-rw-r--r--   0        0        0     3711 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_plans/time_series.py
+-rw-r--r--   0        0        0     1988 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_suites/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/test_suites/test_suites.py
+-rw-r--r--   0        0        0     6769 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/utils.py
+-rw-r--r--   0        0        0     1116 2023-05-14 02:11:48.672362 validmind-1.9.5/validmind/vm_models/__init__.py
+-rw-r--r--   0        0        0    11031 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/dataset.py
+-rw-r--r--   0        0        0     8287 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/dataset_utils.py
+-rw-r--r--   0        0        0      592 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/figure.py
+-rw-r--r--   0        0        0     3746 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/metric.py
+-rw-r--r--   0        0        0     1757 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/metric_result.py
+-rw-r--r--   0        0        0     6530 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/model.py
+-rw-r--r--   0        0        0     3721 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/plot_utils.py
+-rw-r--r--   0        0        0     1518 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/result_summary.py
+-rw-r--r--   0        0        0     2501 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_context.py
+-rw-r--r--   0        0        0    11803 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_plan.py
+-rw-r--r--   0        0        0    18529 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_plan_result.py
+-rw-r--r--   0        0        0     1698 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_result.py
+-rw-r--r--   0        0        0     5019 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/test_suite.py
+-rw-r--r--   0        0        0     3620 2023-05-14 02:11:48.676362 validmind-1.9.5/validmind/vm_models/threshold_test.py
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.5/PKG-INFO
```

### Comparing `validmind-1.9.4/LICENSE` & `validmind-1.9.5/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,64 @@
 SOFTWARE LICENSE AGREEMENT
 
 IMPORTANT - READ CAREFULLY:
 
-This software and associated media, printed materials, and "online" or electronic documentation files (the "Software"), is the proprietary information of ValidMind Inc. and its licensors, and is protected under copyright and other intellectual property laws.
+This software and associated media, printed materials, and "online" or electronic
+documentation files (the "Software"), is the proprietary information of ValidMind Inc. and
+its licensors, and is protected under copyright and other intellectual property laws.
+
+No part of this Software may be copied, reproduced, distributed, republished, downloaded,
+displayed, posted or transmitted in any form or by any means, including, but not limited to,
+electronic, mechanical, photocopying, recording, or otherwise, without the prior written
+permission of ValidMind Inc. or the respective copyright owner.
+
+By installing, copying, or otherwise using the Software, you agree to be bound by the terms
+of this Agreement. If you do not agree to the terms of this Agreement, do not install or use
+the Software.
+
+LICENSE GRANT. Subject to the terms and conditions of this Agreement, Licensor grants you a
+personal, non-exclusive, non-transferable license to use the Software solely for the
+duration of the 4-week testing phase (“Testing”) of the Software - starting on May 15th,
+2023. You may install and use the Software on a single computer or device.
+
+OWNERSHIP. The Software is owned by Licensor and is protected by copyright laws and
+international copyright treaties, as well as other intellectual property laws and treaties.
+Licensor retains all right, title, and interest in and to the Software, including all
+intellectual property rights.
+
+RESTRICTIONS. You may not modify, adapt, translate, reverse engineer, decompile,
+disassemble, or otherwise attempt to discover the source code of the Software including
+(without limitation) for the purpose of obtaining unauthorized access to the Software. You
+may not distribute, sublicense, rent, lease, or lend the Software to any third party.
+
+SUPPORT. Licensor may, at its discretion, provide technical support for the Software.
+Technical support is provided on a best-effort basis and is subject to Licensor's support
+policies.
+
+TERMINATION. This Agreement will terminate automatically after the Testing period, or if you
+fail to comply with any of the terms and conditions of this Agreement. Upon termination, you
+must immediately cease all use of the Software and destroy all copies of the Software in
+your possession.
+
+DISCLAIMER OF WARRANTY. THE SOFTWARE IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND,
+EITHER EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. LICENSOR DOES NOT WARRANT THAT THE
+SOFTWARE WILL MEET YOUR REQUIREMENTS OR THAT OPERATION OF THE SOFTWARE WILL BE UNINTERRUPTED
+OR ERROR-FREE.
+
+LIMITATION OF LIABILITY. IN NO EVENT SHALL LICENSOR BE LIABLE FOR ANY INDIRECT, SPECIAL,
+INCIDENTAL, OR CONSEQUENTIAL DAMAGES ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+INABILITY TO USE THE SOFTWARE, EVEN IF LICENSOR HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGES. IN NO EVENT SHALL LICENSOR'S LIABILITY EXCEED THE AMOUNT PAID BY YOU FOR THE
+SOFTWARE.
+
+GOVERNING LAW. This Agreement shall be governed by and construed in accordance with the laws
+of the United States of America, without giving effect to any principles of conflicts of law.
+
+ENTIRE AGREEMENT. This Agreement constitutes the entire agreement between you and Licensor
+with respect to the Software and supersedes all prior or contemporaneous communications and
+proposals, whether oral or written, between you and Licensor.
 
-No part of this Software may be copied, reproduced, distributed, republished, downloaded, displayed, posted or transmitted in any form or by any means, including, but not limited to, electronic, mechanical, photocopying, recording, or otherwise, without the prior written permission of ValidMind Inc. or the respective copyright owner.
-
-By installing, copying, or otherwise using the Software, you agree to be bound by the terms of this Agreement. If you do not agree to the terms of this Agreement, do not install or use the Software.
-
-LICENSE GRANT. Subject to the terms and conditions of this Agreement, Licensor grants you a personal, non-exclusive, non-transferable license to use the Software solely for the duration of the 4-week testing phase (“Testing”) of the Software - starting on May 15th, 2023. You may install and use the Software on a single computer or device.
-
-OWNERSHIP. The Software is owned by Licensor and is protected by copyright laws and international copyright treaties, as well as other intellectual property laws and treaties. Licensor retains all right, title, and interest in and to the Software, including all intellectual property rights.
-
-RESTRICTIONS. You may not modify, adapt, translate, reverse engineer, decompile, disassemble, or otherwise attempt to discover the source code of the Software including (without limitation) for the purpose of obtaining unauthorized access to the Software. You may not distribute, sublicense, rent, lease, or lend the Software to any third party.
-
-SUPPORT. Licensor may, at its discretion, provide technical support for the Software. Technical support is provided on a best-effort basis and is subject to Licensor's support policies.
-
-TERMINATION. This Agreement will terminate automatically after the Testing period, or if you fail to comply with any of the terms and conditions of this Agreement. Upon termination, you must immediately cease all use of the Software and destroy all copies of the Software in your possession.
-
-DISCLAIMER OF WARRANTY. THE SOFTWARE IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. LICENSOR DOES NOT WARRANT THAT THE SOFTWARE WILL MEET YOUR REQUIREMENTS OR THAT OPERATION OF THE SOFTWARE WILL BE UNINTERRUPTED OR ERROR-FREE.
-
-LIMITATION OF LIABILITY. IN NO EVENT SHALL LICENSOR BE LIABLE FOR ANY INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES ARISING OUT OF OR IN CONNECTION WITH THE USE OR INABILITY TO USE THE SOFTWARE, EVEN IF LICENSOR HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. IN NO EVENT SHALL LICENSOR'S LIABILITY EXCEED THE AMOUNT PAID BY YOU FOR THE SOFTWARE.
-
-GOVERNING LAW. This Agreement shall be governed by and construed in accordance with the laws of the United States of America, without giving effect to any principles of conflicts of law.
-
-ENTIRE AGREEMENT. This Agreement constitutes the entire agreement between you and Licensor with respect to the Software and supersedes all prior or contemporaneous communications and proposals, whether oral or written, between you and Licensor.
-
-By installing or using the Software, you acknowledge that you have read this Agreement, understand it, and agree to be bound by its terms and conditions.
+By installing or using the Software, you acknowledge that you have read this Agreement,
+understand it, and agree to be bound by its terms and conditions.
 
 Copyright © 2023 ValidMind Inc. All rights reserved.
```

### Comparing `validmind-1.9.4/pyproject.toml` & `validmind-1.9.5/pyproject.toml`

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
-version = "1.9.4"
+version = "1.9.5"
 
 [tool.poetry.dependencies]
 arch = "^5.4.0"
 click = "^8.0.4"
 dython = "^0.7.1"
 ipython = "^8.11.0"
 myst-parser = "^1.0.0"
```

### Comparing `validmind-1.9.4/validmind/__init__.py` & `validmind-1.9.5/validmind/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/api_client.py` & `validmind-1.9.5/validmind/api_client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/client.py` & `validmind-1.9.5/validmind/client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/data_validation/__init__.py` & `validmind-1.9.5/validmind/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/data_validation/metrics.py` & `validmind-1.9.5/validmind/data_validation/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from statsmodels.tsa.arima.model import ARIMA
 from statsmodels.tsa.stattools import adfuller
 from statsmodels.tsa.seasonal import seasonal_decompose
 from statsmodels.graphics.tsaplots import plot_acf, plot_pacf
 from statsmodels.tsa.stattools import coint
 
 
+from ..utils import format_records
 from ..vm_models import (
     Figure,
     Metric,
     ResultSummary,
     ResultTable,
     ResultTableMetadata,
     TestContext,
@@ -129,15 +130,16 @@
         summary_stats = self.df[numerical_fields].describe(percentiles=percentiles).T
         summary_stats = summary_stats[
             ["count", "mean", "std", "min", "25%", "50%", "75%", "90%", "95%", "max"]
         ]
         summary_stats.columns = summary_stats.columns.str.title()
         summary_stats.reset_index(inplace=True)
         summary_stats.rename(columns={"index": "Name"}, inplace=True)
-        return summary_stats
+
+        return format_records(summary_stats)
 
     def get_summary_statistics_categorical(self, categorical_fields):
         summary_stats = pd.DataFrame()
         for column in self.df[categorical_fields].columns:
             top_value = self.df[column].value_counts().idxmax()
             top_freq = self.df[column].value_counts().max()
             summary_stats.loc[column, "Count"] = self.df[column].count()
@@ -149,15 +151,15 @@
             summary_stats.loc[column, "Top Value Frequency %"] = (
                 top_freq / self.df[column].count()
             ) * 100
 
         summary_stats.reset_index(inplace=True)
         summary_stats.rename(columns={"index": "Name"}, inplace=True)
 
-        return summary_stats
+        return format_records(summary_stats)
 
     def summary(self, metric_value):
         """
         Build two tables: one for summarizing numerical variables and one for categorical variables
         """
         summary_stats_numerical = metric_value["numerical"]
         summary_stats_categorical = metric_value["categorical"]
@@ -183,16 +185,16 @@
             numerical_fields
         )
         summary_stats_categorical = self.get_summary_statistics_categorical(
             categorical_fields
         )
         return self.cache_results(
             {
-                "numerical": summary_stats_numerical.to_dict(orient="records"),
-                "categorical": summary_stats_categorical.to_dict(orient="records"),
+                "numerical": summary_stats_numerical,
+                "categorical": summary_stats_categorical,
             }
         )
 
 
 class DatasetSplit(Metric):
     """
     Attempts to extract information about the dataset split from the
```

### Comparing `validmind-1.9.4/validmind/data_validation/threshold_tests.py` & `validmind-1.9.5/validmind/data_validation/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/classification/__init__.py` & `validmind-1.9.5/validmind/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/classification/customer_churn.py` & `validmind-1.9.5/validmind/datasets/classification/customer_churn.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/classification/datasets/bank_customer_churn.csv` & `validmind-1.9.5/validmind/datasets/classification/datasets/bank_customer_churn.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/classification/datasets/taiwan_credit.csv` & `validmind-1.9.5/validmind/datasets/classification/datasets/taiwan_credit.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/classification/taiwan_credit.py` & `validmind-1.9.5/validmind/datasets/classification/taiwan_credit.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/__init__.py` & `validmind-1.9.5/validmind/datasets/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates.csv` & `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv` & `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv` & `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv` & `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv` & `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv` & `validmind-1.9.5/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/datasets/lending_club_loan_rates.csv` & `validmind-1.9.5/validmind/datasets/regression/datasets/lending_club_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/fred.py` & `validmind-1.9.5/validmind/datasets/regression/fred.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/lending_club.py` & `validmind-1.9.5/validmind/datasets/regression/lending_club.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl` & `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl` & `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl` & `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl` & `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl` & `validmind-1.9.5/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/model_utils.py` & `validmind-1.9.5/validmind/model_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/model_validation/model_metadata.py` & `validmind-1.9.5/validmind/model_validation/model_metadata.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/model_validation/sklearn/threshold_tests.py` & `validmind-1.9.5/validmind/model_validation/sklearn/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/model_validation/statsmodels/metrics.py` & `validmind-1.9.5/validmind/model_validation/statsmodels/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,16 +560,18 @@
     Test that output the summary of regression models of statsmodel library.
     """
 
     name = "regression_model_summary"
 
     def run(self):
         if not Model.is_supported_model(self.model.model):
-            raise ValueError(f"{Model.model_library(self.model.model)}.{Model.model_class(self.model.model)} \
-                              is not supported by ValidMind framework yet")
+            raise ValueError(
+                f"{Model.model_library(self.model.model)}.{Model.model_class(self.model.model)} \
+                              is not supported by ValidMind framework yet"
+            )
 
         X_columns = self.model.train_ds.get_features_columns()
 
         y_true = self.model.train_ds.y
         y_pred = self.model.model.predict(self.model.train_ds.x)
 
         r2 = r2_score(y_true, y_pred)
@@ -634,16 +636,18 @@
             all_models.append(self.model)
 
         if self.models is not None:
             all_models.extend(self.models)
 
         for m in all_models:
             if not Model.is_supported_model(m.model):
-                raise ValueError(f"{Model.model_library(m.model)}.{Model.model_class(m.model)} \
-                              is not supported by ValidMind framework yet")
+                raise ValueError(
+                    f"{Model.model_library(m.model)}.{Model.model_class(m.model)} \
+                              is not supported by ValidMind framework yet"
+                )
         results = self._in_sample_performance_ols(all_models)
         return self.cache_results(
             {
                 "in_sample_performance": pd.DataFrame(results).to_dict(
                     orient="records"
                 ),
             }
@@ -736,16 +740,18 @@
             all_models.append(self.model)
 
         if self.models is not None:
             all_models.extend(self.models)
 
         for model in all_models:
             if not Model.is_supported_model(model.model):
-                raise ValueError(f"{Model.model_library(model.model)}.{Model.model_class(model.model)} \
-                                is not supported by ValidMind framework yet")
+                raise ValueError(
+                    f"{Model.model_library(model.model)}.{Model.model_class(model.model)} \
+                                is not supported by ValidMind framework yet"
+                )
             if model.test_ds is None:
                 raise ValueError(
                     "Test dataset is missing in the ValidMind Model object"
                 )
 
         results = self._out_sample_performance_ols(
             all_models,
@@ -844,16 +850,18 @@
 
         # Check models list is not empty
         if not self.models:
             raise ValueError("List of models must be provided in the models parameter")
         all_models = []
         for model in self.models:
             if not Model.is_supported_model(model.model):
-                raise ValueError(f"{Model.model_library(model.model)}.{Model.model_class(model.model)} \
-                                 is not supported by ValidMind framework yet")
+                raise ValueError(
+                    f"{Model.model_library(model.model)}.{Model.model_class(model.model)} \
+                                 is not supported by ValidMind framework yet"
+                )
             all_models.append(model)
 
         figures = self._plot_forecast(all_models, start_date, end_date)
 
         return self.cache_results(figures=figures)
 
     def _plot_forecast(self, model_list, start_date=None, end_date=None):
```

### Comparing `validmind-1.9.4/validmind/model_validation/statsmodels/threshold_tests.py` & `validmind-1.9.5/validmind/model_validation/statsmodels/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/model_validation/utils.py` & `validmind-1.9.5/validmind/model_validation/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/test_plans/__init__.py` & `validmind-1.9.5/validmind/test_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/test_plans/binary_classifier.py` & `validmind-1.9.5/validmind/test_plans/binary_classifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,19 @@
 custom test plan from the project's configuration
 """
 
 from ..vm_models import TestPlan
 from ..data_validation.metrics import DatasetSplit
 from ..model_validation.model_metadata import ModelMetadata
 from ..model_validation.sklearn.metrics import (
-    AccuracyScore,
+    ClassifierInSamplePerformance,
+    ClassifierOutOfSamplePerformance,
     ConfusionMatrix,
-    F1Score,
     PermutationFeatureImportance,
     PrecisionRecallCurve,
-    PrecisionScore,
-    RecallScore,
-    ROCAUCScore,
     ROCCurve,
     CharacteristicStabilityIndex,
     PopulationStabilityIndex,
     SHAPGlobalImportance,
 )
 from ..model_validation.sklearn.threshold_tests import (
     MinimumAccuracy,
@@ -39,22 +36,19 @@
     """
 
     name = "binary_classifier_metrics"
     required_context = ["model"]
     tests = [
         ModelMetadata,
         DatasetSplit,
-        AccuracyScore,
         ConfusionMatrix,
-        F1Score,
+        ClassifierInSamplePerformance,
+        ClassifierOutOfSamplePerformance,
         PermutationFeatureImportance,
         PrecisionRecallCurve,
-        PrecisionScore,
-        RecallScore,
-        ROCAUCScore,
         ROCCurve,
         CharacteristicStabilityIndex,
         PopulationStabilityIndex,
         SHAPGlobalImportance,
     ]
```

### Comparing `validmind-1.9.4/validmind/test_plans/statsmodels_timeseries.py` & `validmind-1.9.5/validmind/test_plans/statsmodels_timeseries.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/test_plans/tabular_datasets.py` & `validmind-1.9.5/validmind/test_plans/tabular_datasets.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/test_plans/time_series.py` & `validmind-1.9.5/validmind/test_plans/time_series.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/test_suites/__init__.py` & `validmind-1.9.5/validmind/test_suites/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/test_suites/test_suites.py` & `validmind-1.9.5/validmind/test_suites/test_suites.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/utils.py` & `validmind-1.9.5/validmind/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from IPython.core import getipython
 from numpy import ndarray
 from tabulate import tabulate
 
 
 DEFAULT_BIG_NUMBER_DECIMALS = 2
-DEFAULT_SMALL_NUMBER_DECIMALS = 6
+DEFAULT_SMALL_NUMBER_DECIMALS = 4
 
 
 def nan_to_none(obj):
     if isinstance(obj, dict):
         return {k: nan_to_none(v) for k, v in obj.items()}
     elif isinstance(obj, list):
         return [nan_to_none(v) for v in obj]
@@ -110,14 +110,16 @@
 
     - Check if we are rendering "big" numbers greater than 10 or just numbers between 0 and 1
     - If the column's smallest number has more decimals 6, use that number's precision
       so we can avoid rendering a 0 instead
     - If the column's smallest number has less decimals than 6, use 6 decimal places
     """
     for col in df.columns:
+        if df[col].dtype == "object":
+            continue
         not_zero = df[col][df[col] != 0]
         min_number = not_zero.min()
         _, min_scale = precision_and_scale(min_number)
 
         if min_number >= 10:
             df[col] = df[col].round(DEFAULT_BIG_NUMBER_DECIMALS)
         elif min_scale > DEFAULT_SMALL_NUMBER_DECIMALS:
@@ -199,7 +201,18 @@
     cleandoc = inspect.cleandoc(docstring)
 
     # Replace newlines with spaces, leave double newlines \n\n alone
     pattern = r"(?<!\n)\n(?!\n)"
     replacement = " "
 
     return re.sub(pattern, replacement, cleandoc)
+
+
+def format_number(number):
+    """
+    Format a number for display purposes. If the number is a float, round it
+    to 4 decimal places.
+    """
+    if isinstance(number, float):
+        return round(number, 4)
+    else:
+        return number
```

### Comparing `validmind-1.9.4/validmind/vm_models/__init__.py` & `validmind-1.9.5/validmind/vm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/dataset.py` & `validmind-1.9.5/validmind/vm_models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,17 +140,15 @@
 
         Returns:
             list: The list of features columns
         """
         return [
             field_dic["id"]
             for field_dic in self.fields
-            if (
-                field_dic["id"] != self.target_column
-            )
+            if (field_dic["id"] != self.target_column)
         ]
 
     def get_numeric_features_columns(self):
         """
         Returns list of numeric features columns
 
         Returns:
```

### Comparing `validmind-1.9.4/validmind/vm_models/dataset_utils.py` & `validmind-1.9.5/validmind/vm_models/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/figure.py` & `validmind-1.9.5/validmind/vm_models/figure.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/metric.py` & `validmind-1.9.5/validmind/vm_models/metric.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/metric_result.py` & `validmind-1.9.5/validmind/vm_models/metric_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/model.py` & `validmind-1.9.5/validmind/vm_models/model.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/plot_utils.py` & `validmind-1.9.5/validmind/vm_models/plot_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/result_summary.py` & `validmind-1.9.5/validmind/vm_models/result_summary.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/test_context.py` & `validmind-1.9.5/validmind/vm_models/test_context.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/test_plan.py` & `validmind-1.9.5/validmind/vm_models/test_plan.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/test_plan_result.py` & `validmind-1.9.5/validmind/vm_models/test_plan_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/test_result.py` & `validmind-1.9.5/validmind/vm_models/test_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/test_suite.py` & `validmind-1.9.5/validmind/vm_models/test_suite.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/validmind/vm_models/threshold_test.py` & `validmind-1.9.5/validmind/vm_models/threshold_test.py`

 * *Files identical despite different names*

### Comparing `validmind-1.9.4/PKG-INFO` & `validmind-1.9.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validmind
-Version: 1.9.4
+Version: 1.9.5
 Summary: ValidMind Developer Framework
 Author: Andres Rodriguez
 Author-email: andres@validmind.ai
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

