# Comparing `tmp/pureml-0.3.7.tar.gz` & `tmp/pureml-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml-0.3.7.tar", max compression
+gzip compressed data, was "pureml-0.3.8.tar", max compression
```

## Comparing `pureml-0.3.7.tar` & `pureml-0.3.8.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0    11789 2023-04-27 08:45:08.465073 pureml-0.3.7/README.md
--rw-r--r--   0        0        0      735 2023-05-05 17:31:20.649406 pureml-0.3.7/pureml/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/__init__.py
--rw-r--r--   0        0        0     9746 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/auth.py
--rw-r--r--   0        0        0     2447 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/helpers.py
--rw-r--r--   0        0        0     3201 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/main.py
--rw-r--r--   0        0        0     3365 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/orgs.py
--rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.7/pureml/cli/public.pem
--rw-r--r--   0        0        0     1697 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/puremlconfig.py
--rw-r--r--   0        0        0     7182 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/cli/secrets.py
--rw-r--r--   0        0        0     2861 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/__init__.py
--rw-r--r--   0        0        0     2025 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/auth.py
--rw-r--r--   0        0        0    15074 2023-04-27 20:01:59.833567 pureml-0.3.7/pureml/components/dataset.py
--rw-r--r--   0        0        0       88 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/__init__.py
--rw-r--r--   0        0        0     6866 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/arrays.py
--rw-r--r--   0        0        0     6634 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/artifacts.py
--rw-r--r--   0        0        0     6708 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/audio.py
--rw-r--r--   0        0        0     9603 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/figure.py
--rw-r--r--   0        0        0     6679 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/image.py
--rw-r--r--   0        0        0     2041 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/log.py
--rw-r--r--   0        0        0     5929 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/metrics.py
--rw-r--r--   0        0        0     5925 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/params.py
--rw-r--r--   0        0        0     6166 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/pip_requirement.py
--rw-r--r--   0        0        0     6181 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/predict.py
--rw-r--r--   0        0        0     6049 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/resources.py
--rw-r--r--   0        0        0     6776 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/tabular.py
--rw-r--r--   0        0        0     6168 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/components/log/video.py
--rw-r--r--   0        0        0    13508 2023-04-27 20:02:03.894144 pureml-0.3.7/pureml/components/model.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.7/pureml/config/__init__.py
--rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.7/pureml/config/parser.py
--rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.7/pureml/decorators/__init__.py
--rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.7/pureml/decorators/dataset.py
--rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.7/pureml/decorators/load_data.py
--rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.7/pureml/decorators/model.py
--rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.7/pureml/decorators/pip_requirements.py
--rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.7/pureml/decorators/predict.py
--rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.7/pureml/decorators/transformer.py
--rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.7/pureml/evaluate/__init__.py
--rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.7/pureml/evaluate/classification.py
--rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.7/pureml/evaluate/eval.py
--rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.7/pureml/evaluate/grade.py
--rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.7/pureml/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.7/pureml/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.7/pureml/evaluate/metrics/base.py
--rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.7/pureml/evaluate/metrics/confusion_matrix.py
--rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.7/pureml/evaluate/metrics/f1.py
--rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.7/pureml/evaluate/metrics/mae.py
--rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.7/pureml/evaluate/metrics/mse.py
--rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.7/pureml/evaluate/metrics/precision.py
--rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.7/pureml/evaluate/metrics/recall.py
--rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.7/pureml/evaluate/metrics/roc_auc.py
--rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.7/pureml/evaluate/regression.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.7/pureml/lineage/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.7/pureml/lineage/data/__init__.py
--rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.7/pureml/lineage/data/create_lineage.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.7/pureml/package/__init__.py
--rw-r--r--   0        0        0     6446 2023-04-30 20:33:34.175641 pureml-0.3.7/pureml/package/docker.py
--rw-r--r--   0        0        0     6244 2023-05-05 17:28:39.229763 pureml-0.3.7/pureml/package/fastapi.py
--rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.7/pureml/packaging/__init__.py
--rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/errors.py
--rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_framework.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/__init__.py
--rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/catboost.py
--rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/custom.py
--rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/keras.py
--rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/lightgbm.py
--rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/pytorch.py
--rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/pytorch_tabnet.py
--rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/sklearn.py
--rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/tensorflow.py
--rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/model_packaging/xgboost.py
--rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.7/pureml/packaging/packaging.py
--rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/packaging/packaging_utils.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.7/pureml/predictor/__init__.py
--rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.7/pureml/predictor/predictor.py
--rw-r--r--   0        0        0      439 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/schema/__init__.py
--rw-r--r--   0        0        0     2580 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/schema/backend.py
--rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.7/pureml/schema/config.py
--rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.7/pureml/schema/dataset.py
--rw-r--r--   0        0        0      163 2023-04-27 08:45:08.465073 pureml-0.3.7/pureml/schema/env.py
--rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/schema/log.py
--rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.7/pureml/schema/model.py
--rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.7/pureml/schema/packaging.py
--rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.7/pureml/schema/paths.py
--rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.7/pureml/schema/predict.py
--rw-r--r--   0        0        0      308 2023-04-27 08:45:08.469073 pureml-0.3.7/pureml/schema/request.py
--rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.7/pureml/schema/singleton.py
--rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/schema/storage.py
--rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.7/pureml/schema/types.py
--rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/settings/__init__.py
--rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/settings/backend.py
--rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/settings/storage.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.7/pureml/utils/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.7/pureml/utils/config.py
--rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.7/pureml/utils/constants.py
--rw-r--r--   0        0        0     1230 2023-04-27 08:45:08.469073 pureml-0.3.7/pureml/utils/env.py
--rw-r--r--   0        0        0     2942 2023-04-27 08:45:08.469073 pureml-0.3.7/pureml/utils/hash.py
--rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.7/pureml/utils/log_utils.py
--rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.7/pureml/utils/package.py
--rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.7/pureml/utils/pipeline.py
--rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.7/pureml/utils/predict.py
--rw-r--r--   0        0        0      816 2023-04-27 08:45:08.469073 pureml-0.3.7/pureml/utils/readme.py
--rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.7/pureml/utils/resources.py
--rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.7/pureml/utils/source_code.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.7/pureml/utils/types.py
--rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.7/pureml/utils/version_utils.py
--rw-r--r--   0        0        0     1927 2023-05-05 17:31:25.116351 pureml-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    13710 1970-01-01 00:00:00.000000 pureml-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11789 2023-04-27 08:45:08.465073 pureml-0.3.8/README.md
+-rw-r--r--   0        0        0      735 2023-05-14 12:52:56.701682 pureml-0.3.8/pureml/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/cli/__init__.py
+-rw-r--r--   0        0        0     9742 2023-05-14 12:52:56.705682 pureml-0.3.8/pureml/cli/auth.py
+-rw-r--r--   0        0        0     2285 2023-05-14 12:52:56.717682 pureml-0.3.8/pureml/cli/helpers.py
+-rw-r--r--   0        0        0     3255 2023-05-14 12:52:56.725683 pureml-0.3.8/pureml/cli/main.py
+-rw-r--r--   0        0        0     3365 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/cli/orgs.py
+-rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.8/pureml/cli/public.pem
+-rw-r--r--   0        0        0     1697 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/cli/puremlconfig.py
+-rw-r--r--   0        0        0     7182 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/cli/secrets.py
+-rw-r--r--   0        0        0     2754 2023-05-14 12:52:56.737684 pureml-0.3.8/pureml/components/__init__.py
+-rw-r--r--   0        0        0     1829 2023-05-14 12:52:56.741684 pureml-0.3.8/pureml/components/auth.py
+-rw-r--r--   0        0        0    15074 2023-05-07 10:40:19.558251 pureml-0.3.8/pureml/components/dataset.py
+-rw-r--r--   0        0        0       88 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/__init__.py
+-rw-r--r--   0        0        0     6866 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/arrays.py
+-rw-r--r--   0        0        0     6634 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/artifacts.py
+-rw-r--r--   0        0        0     6708 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/audio.py
+-rw-r--r--   0        0        0     9603 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/figure.py
+-rw-r--r--   0        0        0     6679 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/image.py
+-rw-r--r--   0        0        0     2041 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/log.py
+-rw-r--r--   0        0        0     5929 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/metrics.py
+-rw-r--r--   0        0        0     5925 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/params.py
+-rw-r--r--   0        0        0     6166 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/pip_requirement.py
+-rw-r--r--   0        0        0     6181 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/predict.py
+-rw-r--r--   0        0        0     6049 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/resources.py
+-rw-r--r--   0        0        0     6776 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/tabular.py
+-rw-r--r--   0        0        0     6168 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/video.py
+-rw-r--r--   0        0        0    13508 2023-05-07 10:40:19.558251 pureml-0.3.8/pureml/components/model.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.8/pureml/config/__init__.py
+-rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.8/pureml/config/parser.py
+-rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.8/pureml/decorators/__init__.py
+-rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.8/pureml/decorators/dataset.py
+-rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.8/pureml/decorators/load_data.py
+-rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.8/pureml/decorators/model.py
+-rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.8/pureml/decorators/pip_requirements.py
+-rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.8/pureml/decorators/predict.py
+-rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.8/pureml/decorators/transformer.py
+-rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.8/pureml/evaluate/__init__.py
+-rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.8/pureml/evaluate/classification.py
+-rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.8/pureml/evaluate/eval.py
+-rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.8/pureml/evaluate/grade.py
+-rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.8/pureml/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.8/pureml/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.8/pureml/evaluate/metrics/base.py
+-rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.8/pureml/evaluate/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.8/pureml/evaluate/metrics/f1.py
+-rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.8/pureml/evaluate/metrics/mae.py
+-rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.8/pureml/evaluate/metrics/mse.py
+-rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.8/pureml/evaluate/metrics/precision.py
+-rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.8/pureml/evaluate/metrics/recall.py
+-rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.8/pureml/evaluate/metrics/roc_auc.py
+-rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.8/pureml/evaluate/regression.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.8/pureml/lineage/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.8/pureml/lineage/data/__init__.py
+-rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.8/pureml/lineage/data/create_lineage.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.8/pureml/package/__init__.py
+-rw-r--r--   0        0        0     6446 2023-04-30 20:33:34.175641 pureml-0.3.8/pureml/package/docker.py
+-rw-r--r--   0        0        0     6189 2023-05-14 12:52:56.749684 pureml-0.3.8/pureml/package/fastapi.py
+-rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.8/pureml/packaging/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/errors.py
+-rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_framework.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/__init__.py
+-rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/catboost.py
+-rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/custom.py
+-rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/keras.py
+-rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/lightgbm.py
+-rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/pytorch.py
+-rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/pytorch_tabnet.py
+-rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/sklearn.py
+-rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/tensorflow.py
+-rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/xgboost.py
+-rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.8/pureml/packaging/packaging.py
+-rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/packaging_utils.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.8/pureml/predictor/__init__.py
+-rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.8/pureml/predictor/predictor.py
+-rw-r--r--   0        0        0      439 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/schema/__init__.py
+-rw-r--r--   0        0        0     2580 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/schema/backend.py
+-rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.8/pureml/schema/config.py
+-rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.8/pureml/schema/dataset.py
+-rw-r--r--   0        0        0      140 2023-05-14 12:52:56.749684 pureml-0.3.8/pureml/schema/env.py
+-rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/schema/log.py
+-rw-r--r--   0        0        0      396 2023-05-14 12:52:47.673188 pureml-0.3.8/pureml/schema/model.py
+-rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.8/pureml/schema/packaging.py
+-rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.8/pureml/schema/paths.py
+-rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.8/pureml/schema/predict.py
+-rw-r--r--   0        0        0      308 2023-04-27 08:45:08.469073 pureml-0.3.8/pureml/schema/request.py
+-rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.8/pureml/schema/singleton.py
+-rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/schema/storage.py
+-rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.8/pureml/schema/types.py
+-rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/settings/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/settings/backend.py
+-rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/settings/storage.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/utils/config.py
+-rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.8/pureml/utils/constants.py
+-rw-r--r--   0        0        0     1044 2023-05-14 12:52:56.761685 pureml-0.3.8/pureml/utils/env.py
+-rw-r--r--   0        0        0     2942 2023-04-27 08:45:08.469073 pureml-0.3.8/pureml/utils/hash.py
+-rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.8/pureml/utils/log_utils.py
+-rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.8/pureml/utils/package.py
+-rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.8/pureml/utils/pipeline.py
+-rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.8/pureml/utils/predict.py
+-rw-r--r--   0        0        0      816 2023-04-27 08:45:08.469073 pureml-0.3.8/pureml/utils/readme.py
+-rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.8/pureml/utils/resources.py
+-rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.8/pureml/utils/source_code.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.8/pureml/utils/types.py
+-rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.8/pureml/utils/version_utils.py
+-rw-r--r--   0        0        0     1927 2023-05-14 12:52:56.765685 pureml-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    13710 1970-01-01 00:00:00.000000 pureml-0.3.8/PKG-INFO
```

### Comparing `pureml-0.3.7/README.md` & `pureml-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/__init__.py` & `pureml-0.3.8/pureml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 from .package import docker, fastapi
 
 from .schema import Input, Output
 from .predictor.predictor import BasePredictor
 
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
```

### Comparing `pureml-0.3.7/pureml/cli/auth.py` & `pureml-0.3.8/pureml/cli/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,19 @@
 def details():
     token = get_token()
     api_token = get_api_token()
     org_id = get_org_id()
 
     print("Org Id: ", org_id)
     if token is not None:
-        print("Access Token: ", token)
+        # print("Access Token: ", token)
+        print("Logged in using access token")
     if api_token is not None:
-        print("API Id: ", api_token["api_id"])
-        print("API Key: ", api_token["api_key"])
+        # print("API Key: ", api_token["api_token"])
+        print("Logged in using API token")
 
 
 @app.callback()
 def callback():
     """
     Authentication user command
 
@@ -131,15 +132,15 @@
     ),
     browserless: bool = typer.Option(
         False, "--browserless", "-s", help="Browserless login for ssh or pipelines"
     ),
     interactive: bool = typer.Option(
         False, "--interactive", "-i", help="Login with email and password interactively"
     ),
-    api_key: bool = typer.Option(False, "--api-key", "-k", help="Login with api key"),
+    api_token: bool = typer.Option(False, "--api-token", "-t", help="Login with api token"),
 ):
     try:
         backend_base_url = get_backend_base_url(backend_url)
         frontend_base_url = get_frontend_base_url(frontend_url)
         # Interactive login with email and password
         if interactive:
             print(f"\n[Enter your credentials to login[/\n")
@@ -166,19 +167,18 @@
                 # Select organization
                 select()
 
             else:
                 print(f"[red]Unable to login to your account!")
 
         # API key login
-        elif api_key:
+        elif api_token:
             print(f"\n[Enter your credentials to login[/\n")
-            api_id: str = typer.prompt("Enter your api id")
-            api_key: str = typer.prompt("Enter your api key")
-            save_auth(api_id=api_id, api_key=api_key)
+            api_token: str = typer.prompt("Enter your api token secret")
+            save_auth(api_token=api_token)
             select()
 
         # Browser based login
         else:
             # Get device details
             device = platform.platform()
             device_data = get_location()
```

### Comparing `pureml-0.3.7/pureml/cli/helpers.py` & `pureml-0.3.8/pureml/cli/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 path_schema = PathSchema().get_instance()
 
 
 def save_auth(
     org_id: str = None,
     access_token: str = None,
     email: str = None,
-    api_id: str = None,
-    api_key: str = None,
+    api_token: str = None,
 ):
     token_path = path_schema.PATH_USER_TOKEN
 
     token_dir = os.path.dirname(token_path)
     os.makedirs(token_dir, exist_ok=True)
 
     # Read existing token
@@ -26,29 +25,26 @@
         with open(token_path, "r") as token_file:
             token = json.load(token_file)
 
         if org_id is not None:
             token["org_id"] = org_id
         if access_token is not None:
             token["accessToken"] = access_token
-        if api_id is not None:
-            token["api_id"] = api_id
-        if api_key is not None:
-            token["api_key"] = api_key
+        if api_token is not None:
+            token["api_token"] = api_token
         if email is not None:
             if "email" in token and token["email"] != email:
                 token["org_id"] = ""
             token["email"] = email
     else:
         token = {
             "org_id": org_id,
             "accessToken": access_token,
             "email": email,
-            "api_id": api_id,
-            "api_key": api_key,
+            "api_token": api_token,
         }
         if org_id is None:
             token["org_id"] = ""
 
     token = json.dumps(token)
 
     with open(token_path, "w") as token_file:
@@ -78,11 +74,10 @@
             headers["Accept"] = accept.value
 
         if token is not None:
             headers["Authorization"] = "Bearer {}".format(token)
             return headers
 
         if api_token is not None:
-            headers["X-Api-Id"] = api_token["api_id"]
-            headers["X-Api-Key"] = api_token["api_key"]
+            headers["X-Api-Key"] = api_token["api_token"]
 
             return headers
```

### Comparing `pureml-0.3.7/pureml/cli/main.py` & `pureml-0.3.8/pureml/cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 import typer
 from pureml.cli.puremlconfig import PureMLConfigYML
-from pureml.config.parser import Config
-# from pureml.trainer.train import Trainer
-import os
-
-app = typer.Typer()
-
-
 import typer
 from rich import print
 # from puretrainer.train import Trainer
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 
 import pureml.cli.auth as auth
 import pureml.cli.secrets as secrets
 import pureml.cli.orgs as orgs
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True)
 app.add_typer(auth.app, name="auth")
 app.add_typer(secrets.app, name="secrets")
 app.add_typer(orgs.app, name="orgs")
 
 
-@app.callback(no_args_is_help=True)
-def validate_user_authentication(ctx: typer.Context):
-    # print(ctx.invoked_subcommand)
-    if ctx.invoked_subcommand in ['auth']:
-        return
-    # user_token = auth.auth_validate()
-    return
+def print_version(value: bool):
+    if value:
+        from pureml import __version__
+
+        print(f"PureML SDK version: {__version__}")
+        raise typer.Exit()
+
+
+@app.callback()
+def callback(
+    version: bool = typer.Option(
+        None, "--version", "-v", callback=print_version, is_eager=True
+    ),
+):
+    """
+    PureML CLI
+
+    This is the official CLI for PureML.
+    """
 
 
 # init the config file
 @app.command()
 def init(
     silent: bool = typer.Option(
         False, "--silent", "-s", help="Run in silent mode"
```

### Comparing `pureml-0.3.7/pureml/cli/orgs.py` & `pureml-0.3.8/pureml/cli/orgs.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/cli/puremlconfig.py` & `pureml-0.3.8/pureml/cli/puremlconfig.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/cli/secrets.py` & `pureml-0.3.8/pureml/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/__init__.py` & `pureml-0.3.8/pureml/components/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,29 +29,27 @@
 def get_api_token():
     """It checks if the api token exists in the user's home directory. If it does, it returns the api token id and key. If it
     doesn't, it returns None
 
     Returns
     -------
         The api token id and key is returned.
-        Dictionary format: {"api_id": api_id, "api_key": api_key}
+        Dictionary format: {"api_token": api_token}
     """
     path = path_schema.PATH_USER_TOKEN
     # path = os.path.expanduser(path)
 
     if os.path.exists(path):
         creds = open(path, "r").read()
 
         creds_json = json.loads(creds)
-        if "api_id" in creds_json and "api_key" in creds_json:
-            api_id = creds_json["api_id"]
-            api_key = creds_json["api_key"]
+        if "api_token" in creds_json:
+            api_token = creds_json["api_token"]
             return {
-                "api_id": api_id,
-                "api_key": api_key
+                "api_token": api_token
             }
     return
 
 
 def delete_token(silent=False):
     """It checks if the token exists in the user's home directory. If it does, it deletes the token. If it
     doesn't, it returns None
```

### Comparing `pureml-0.3.7/pureml/components/auth.py` & `pureml-0.3.8/pureml/components/auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,56 +5,52 @@
 from pureml.cli.auth import save_auth
 from . import delete_token, get_api_token, get_org_id
 from pureml.schema import BackendSchema
 
 backend_schema = BackendSchema().get_instance()
 
 
-def login(org_id: str, api_id: str, api_key: str) -> str:
+def login(org_id: str, api_token: str) -> str:
     """The function takes in a user API token and logs in a user for a session.
 
     Parameters
     ----------
-    api_id: str
-        API Id of the token to be used for login (format: 12345678-1234-1234-1234-123456789012)
-    api_key: str
+    api_token: str
         API Key of the token to be used for login
 
     """
 
     url_path_1 = "org/id/{}".format(org_id)
     url = urljoin(backend_schema.BASE_URL, url_path_1)
 
     if (
-        api_id is None
-        or api_key is None
+        api_token is None
         or org_id is None
-        or api_id == ""
-        or api_key == ""
+        or api_token == ""
         or org_id == ""
     ):
         print("[red]Invalid credentials for login")
         return
 
-    headers = {"X-Api-Id": api_id, "X-Api-Key": api_key}
+    headers = {"X-Api-Key": api_token}
 
     response = requests.get(url, headers=headers)
 
     # print(response.text)
     if response.status_code == 200:
 
         response_text = response.text
         response_org_details = json.loads(response_text)["data"]
 
         # if response_org_details is not None:
         response_org_id = response_org_details[0]["uuid"]
 
         if response_org_id == org_id:
             print("[green]Valid Org Id and API token. Logged in successfully")
-            save_auth(org_id=org_id, api_id=api_id, api_key=api_key)
+            save_auth(org_id=org_id, api_token=api_token)
 
         else:
             print("[orange]Valid Org Id and API token. Obtained different organization")
 
         # else:
         #     print('[green] Invalid Org Id and Access token')
     elif response.status_code == 403:
```

### Comparing `pureml-0.3.7/pureml/components/dataset.py` & `pureml-0.3.8/pureml/components/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/arrays.py` & `pureml-0.3.8/pureml/components/log/arrays.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/artifacts.py` & `pureml-0.3.8/pureml/components/log/artifacts.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/audio.py` & `pureml-0.3.8/pureml/components/log/audio.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/figure.py` & `pureml-0.3.8/pureml/components/log/figure.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/image.py` & `pureml-0.3.8/pureml/components/log/image.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/log.py` & `pureml-0.3.8/pureml/components/log/log.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/metrics.py` & `pureml-0.3.8/pureml/components/log/metrics.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/params.py` & `pureml-0.3.8/pureml/components/log/params.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/pip_requirement.py` & `pureml-0.3.8/pureml/components/log/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/predict.py` & `pureml-0.3.8/pureml/components/log/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/resources.py` & `pureml-0.3.8/pureml/components/log/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/tabular.py` & `pureml-0.3.8/pureml/components/log/tabular.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/log/video.py` & `pureml-0.3.8/pureml/components/log/video.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/components/model.py` & `pureml-0.3.8/pureml/components/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/config/parser.py` & `pureml-0.3.8/pureml/config/parser.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/decorators/dataset.py` & `pureml-0.3.8/pureml/decorators/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/decorators/load_data.py` & `pureml-0.3.8/pureml/decorators/load_data.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/decorators/model.py` & `pureml-0.3.8/pureml/decorators/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/decorators/pip_requirements.py` & `pureml-0.3.8/pureml/decorators/pip_requirements.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/decorators/predict.py` & `pureml-0.3.8/pureml/decorators/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/decorators/transformer.py` & `pureml-0.3.8/pureml/decorators/transformer.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/classification.py` & `pureml-0.3.8/pureml/evaluate/classification.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/eval.py` & `pureml-0.3.8/pureml/evaluate/eval.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/grade.py` & `pureml-0.3.8/pureml/evaluate/grade.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/metrics/accuracy.py` & `pureml-0.3.8/pureml/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/metrics/confusion_matrix.py` & `pureml-0.3.8/pureml/evaluate/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/metrics/f1.py` & `pureml-0.3.8/pureml/evaluate/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/metrics/mae.py` & `pureml-0.3.8/pureml/evaluate/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/metrics/mse.py` & `pureml-0.3.8/pureml/evaluate/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/metrics/precision.py` & `pureml-0.3.8/pureml/evaluate/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/metrics/recall.py` & `pureml-0.3.8/pureml/evaluate/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/metrics/roc_auc.py` & `pureml-0.3.8/pureml/evaluate/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/evaluate/regression.py` & `pureml-0.3.8/pureml/evaluate/regression.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/lineage/data/create_lineage.py` & `pureml-0.3.8/pureml/lineage/data/create_lineage.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/package/docker.py` & `pureml-0.3.8/pureml/package/docker.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/package/fastapi.py` & `pureml-0.3.8/pureml/package/fastapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,19 +100,18 @@
 
 import nest_asyncio
 from pyngrok import ngrok
 
 load_dotenv()
 
 org_id = os.getenv('ORG_ID')
-api_id = os.getenv('API_ID')
-api_key = os.getenv('API_KEY')
+api_token = os.getenv('API_TOKEN')
 
-if api_id is not None and api_key is not None and org_id is not None:
-    pureml.login(org_id=org_id, api_id=api_id, api_key=api_key)
+if api_token is not None and org_id is not None:
+    pureml.login(org_id=org_id, api_token=api_token)
 
 predictor = Predictor()
 predictor.load_models()
 
 # input_type, input_shape = process_input(input=predictor.input)
 # output_type, output_shape = process_output(output=predictor.output)
 
@@ -197,15 +196,15 @@
         label, predict_path=predict_path, requirements_path=requirements_path
     )
 
     interpreter_path = str(sys.executable)
 
     if os.path.exists(interpreter_path):
 
-        run_command = "{interpreter_path} '{api_path}'".format(
+        run_command = "'{interpreter_path}' '{api_path}'".format(
             interpreter_path=interpreter_path, api_path=fastapi_schema.PATH_FASTAPI_FILE
         )
 
         os.system(run_command)
     else:
         print("Interpreter not found at", interpreter_path)
```

### Comparing `pureml-0.3.7/pureml/packaging/__init__.py` & `pureml-0.3.8/pureml/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_framework.py` & `pureml-0.3.8/pureml/packaging/model_framework.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/catboost.py` & `pureml-0.3.8/pureml/packaging/model_packaging/catboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/custom.py` & `pureml-0.3.8/pureml/packaging/model_packaging/custom.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/keras.py` & `pureml-0.3.8/pureml/packaging/model_packaging/keras.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/lightgbm.py` & `pureml-0.3.8/pureml/packaging/model_packaging/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/pytorch.py` & `pureml-0.3.8/pureml/packaging/model_packaging/pytorch.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/pytorch_tabnet.py` & `pureml-0.3.8/pureml/packaging/model_packaging/pytorch_tabnet.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/sklearn.py` & `pureml-0.3.8/pureml/packaging/model_packaging/sklearn.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/tensorflow.py` & `pureml-0.3.8/pureml/packaging/model_packaging/tensorflow.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/model_packaging/xgboost.py` & `pureml-0.3.8/pureml/packaging/model_packaging/xgboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/packaging.py` & `pureml-0.3.8/pureml/packaging/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/packaging/packaging_utils.py` & `pureml-0.3.8/pureml/packaging/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/predictor/predictor.py` & `pureml-0.3.8/pureml/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/schema/backend.py` & `pureml-0.3.8/pureml/schema/backend.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/schema/packaging.py` & `pureml-0.3.8/pureml/schema/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/schema/paths.py` & `pureml-0.3.8/pureml/schema/paths.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/schema/predict.py` & `pureml-0.3.8/pureml/schema/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/config.py` & `pureml-0.3.8/pureml/utils/config.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/constants.py` & `pureml-0.3.8/pureml/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/env.py` & `pureml-0.3.8/pureml/utils/env.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,43 +5,37 @@
 
 
 def generate_env_dict(env_path):
     load_dotenv(dotenv_path=env_path)
 
     org_id = os.getenv(Env.ORG_ID.value)
     access_token = os.getenv(Env.ACCESS_TOKEN.value)
-    api_id = os.getenv(Env.API_ID.value)
-    api_key = os.getenv(Env.API_KEY.value)
+    api_token = os.getenv(Env.API_TOKEN.value)
 
     env_dict = {}
 
     if org_id is None:
         print("[red]", Env.ORG_ID.value, "is not set in .env")
     else:
         env_dict[Env.ORG_ID.value] = org_id
 
     if access_token is None:
         print("[red]", Env.ACCESS_TOKEN.value, "is not set in .env")
     else:
         env_dict[Env.ACCESS_TOKEN.value] = access_token
 
-    if api_id is None:
-        print("[red]", Env.API_ID.value, "is not set in .env")
+    if api_token is None:
+        print("[red]", Env.API_TOKEN.value, "is not set in .env")
     else:
-        env_dict[Env.API_ID.value] = api_id
-
-    if api_key is None:
-        print("[red]", Env.API_KEY.value, "is not set in .env")
-    else:
-        env_dict[Env.API_KEY.value] = api_key
+        env_dict[Env.API_TOKEN.value] = api_token
 
     return env_dict
 
 
 def validate_env_docker(env_dict):
     env_dict_set = set(list(env_dict.keys()))
-    env_dict_docker = set([Env.ORG_ID.value, Env.API_ID.value, Env.API_KEY.value])
+    env_dict_docker = set([Env.ORG_ID.value, Env.API_TOKEN.value])
 
     if env_dict_docker.issubset(env_dict_set):
         return True
 
     return False
```

### Comparing `pureml-0.3.7/pureml/utils/hash.py` & `pureml-0.3.8/pureml/utils/hash.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/log_utils.py` & `pureml-0.3.8/pureml/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/package.py` & `pureml-0.3.8/pureml/utils/package.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/pipeline.py` & `pureml-0.3.8/pureml/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/predict.py` & `pureml-0.3.8/pureml/utils/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/readme.py` & `pureml-0.3.8/pureml/utils/readme.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/resources.py` & `pureml-0.3.8/pureml/utils/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pureml/utils/version_utils.py` & `pureml-0.3.8/pureml/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.7/pyproject.toml` & `pureml-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml"
-version = "0.3.7"
+version = "0.3.8"
 description = ""
 license = "Apache-2.0"
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 homepage = "https://pureml.com/"
 repository = "https://github.com/engageml-github/Pure"
 documentation = "https://docs.pureml.com"
```

### Comparing `pureml-0.3.7/PKG-INFO` & `pureml-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pureml
-Version: 0.3.7
+Version: 0.3.8
 Summary: 
 Home-page: https://pureml.com/
 License: Apache-2.0
 Keywords: pureml,model-store,machine-learning,python,model-registry,collabortion
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.8,<4.0
```

