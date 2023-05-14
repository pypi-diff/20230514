# Comparing `tmp/kiwi_booster-0.1.0.tar.gz` & `tmp/kiwi_booster-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwi_booster-0.1.0.tar", max compression
+gzip compressed data, was "kiwi_booster-0.2.0.tar", max compression
```

## Comparing `kiwi_booster-0.1.0.tar` & `kiwi_booster-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-05-10 16:09:22.014857 kiwi_booster-0.1.0/LICENSE
--rw-r--r--   0        0        0       46 2023-05-10 16:09:22.014857 kiwi_booster-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-10 16:49:56.868768 kiwi_booster-0.1.0/kiwi_booster/__init__.py
--rw-r--r--   0        0        0     3860 2023-05-11 15:23:01.518525 kiwi_booster-0.1.0/kiwi_booster/slack_bot.py
--rw-r--r--   0        0        0      406 2023-05-11 15:36:05.856385 kiwi_booster-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 kiwi_booster-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 16:09:22.014857 kiwi_booster-0.2.0/LICENSE
+-rw-r--r--   0        0        0       46 2023-05-10 16:09:22.014857 kiwi_booster-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 15:53:32.721294 kiwi_booster-0.2.0/kiwi_booster/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 16:06:23.304697 kiwi_booster-0.2.0/kiwi_booster/common_utils/__init__.py
+-rw-r--r--   0        0        0      179 2023-05-14 16:06:24.796208 kiwi_booster-0.2.0/kiwi_booster/common_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1405 2023-05-14 16:06:24.796208 kiwi_booster-0.2.0/kiwi_booster/common_utils/__pycache__/loggers.cpython-310.pyc
+-rw-r--r--   0        0        0     1748 2023-05-14 16:09:16.985180 kiwi_booster-0.2.0/kiwi_booster/common_utils/loggers.py
+-rw-r--r--   0        0        0     1455 2023-05-14 16:08:18.524135 kiwi_booster-0.2.0/kiwi_booster/common_utils/mixed.py
+-rw-r--r--   0        0        0        0 2023-05-11 22:59:08.795321 kiwi_booster-0.2.0/kiwi_booster/common_utils/requests.py
+-rw-r--r--   0        0        0     1686 2023-05-14 16:09:16.981179 kiwi_booster-0.2.0/kiwi_booster/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.2.0/kiwi_booster/gcp_utils/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-14 16:08:00.494154 kiwi_booster-0.2.0/kiwi_booster/gcp_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1938 2023-05-14 16:08:00.494154 kiwi_booster-0.2.0/kiwi_booster/gcp_utils/__pycache__/storage.cpython-310.pyc
+-rw-r--r--   0        0        0      510 2023-05-14 16:08:18.508133 kiwi_booster-0.2.0/kiwi_booster/gcp_utils/bigquery.py
+-rw-r--r--   0        0        0      567 2023-05-11 23:22:34.716563 kiwi_booster-0.2.0/kiwi_booster/gcp_utils/kfp.py
+-rw-r--r--   0        0        0     2038 2023-05-14 16:09:16.989180 kiwi_booster-0.2.0/kiwi_booster/gcp_utils/secrets.py
+-rw-r--r--   0        0        0     1803 2023-05-14 16:09:16.985180 kiwi_booster-0.2.0/kiwi_booster/gcp_utils/storage.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.2.0/kiwi_booster/ml_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:00:22.783840 kiwi_booster-0.2.0/kiwi_booster/ml_utils/benchmarks.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:00:10.175752 kiwi_booster-0.2.0/kiwi_booster/ml_utils/prediction.py
+-rw-r--r--   0        0        0     3859 2023-05-14 16:08:18.540137 kiwi_booster-0.2.0/kiwi_booster/slack_utils.py
+-rw-r--r--   0        0        0      687 2023-05-14 16:11:10.016776 kiwi_booster-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 kiwi_booster-0.2.0/PKG-INFO
```

### Comparing `kiwi_booster-0.1.0/LICENSE` & `kiwi_booster-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.1.0/kiwi_booster/slack_bot.py` & `kiwi_booster-0.2.0/kiwi_booster/slack_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         block = []
         color = (
             self.color_map[type]
             if type in self.color_map.keys()
             else self.color_map["info"]
         )
         for type, message in kwargs.items():
-
             block.append(
                 {
                     "color": f"{color}",
                     "blocks": [
                         {
                             "type": "section",
                             "text": {
```

