# Comparing `tmp/quant_invest_lab-0.2.0.tar.gz` & `tmp/quant_invest_lab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_lab-0.2.0.tar", max compression
+gzip compressed data, was "quant_invest_lab-0.2.1.tar", max compression
```

## Comparing `quant_invest_lab-0.2.0.tar` & `quant_invest_lab-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1994 2023-05-14 18:11:45.604751 quant_invest_lab-0.2.0/README.md
--rw-r--r--   0        0        0      978 2023-05-14 18:14:19.404751 quant_invest_lab-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    18278 2023-05-14 17:42:39.234752 quant_invest_lab-0.2.0/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0    17111 2023-05-14 17:05:21.454752 quant_invest_lab-0.2.0/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    19099 2023-05-14 17:22:56.994752 quant_invest_lab-0.2.0/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0     8038 2023-05-14 15:47:17.294752 quant_invest_lab-0.2.0/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0    20361 2023-05-14 18:09:36.804750 quant_invest_lab-0.2.0/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-14 17:30:20.244749 quant_invest_lab-0.2.0/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     8477 2023-05-14 17:22:27.984752 quant_invest_lab-0.2.0/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0     1107 2023-05-14 17:21:39.694751 quant_invest_lab-0.2.0/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     3280 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.0/setup.py
--rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4427 2023-05-14 20:28:40.324711 quant_invest_lab-0.2.1/README.md
+-rw-r--r--   0        0        0      978 2023-05-14 20:22:51.144752 quant_invest_lab-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    18278 2023-05-14 17:42:39.234752 quant_invest_lab-0.2.1/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0    17111 2023-05-14 17:05:21.454752 quant_invest_lab-0.2.1/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    26223 2023-05-14 20:20:38.384760 quant_invest_lab-0.2.1/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0     8038 2023-05-14 15:47:17.294752 quant_invest_lab-0.2.1/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0     7659 2023-05-14 20:17:42.054696 quant_invest_lab-0.2.1/quant_invest_lab/optimization.py
+-rw-r--r--   0        0        0    20361 2023-05-14 18:09:36.804750 quant_invest_lab-0.2.1/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-14 17:30:20.244749 quant_invest_lab-0.2.1/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     8477 2023-05-14 17:22:27.984752 quant_invest_lab-0.2.1/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0     1107 2023-05-14 17:21:39.694751 quant_invest_lab-0.2.1/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     5790 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.1/setup.py
+-rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.1/PKG-INFO
```

### Comparing `quant_invest_lab-0.2.0/pyproject.toml` & `quant_invest_lab-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quant-invest-lab"
-version = "0.2.0"
+version = "0.2.1"
 description = "Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project."
 authors = ["BaptisteZloch <bzloch@hotmail.fr>"]
 readme = "README.md"
 packages = [{include = "quant_invest_lab"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `quant_invest_lab-0.2.0/quant_invest_lab/backtest.py` & `quant_invest_lab-0.2.1/quant_invest_lab/backtest.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.0/quant_invest_lab/data_provider.py` & `quant_invest_lab-0.2.1/quant_invest_lab/data_provider.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.0/quant_invest_lab/metrics.py` & `quant_invest_lab-0.2.1/quant_invest_lab/metrics.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.0/quant_invest_lab/portfolio.py` & `quant_invest_lab-0.2.1/quant_invest_lab/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.0/quant_invest_lab/screener.py` & `quant_invest_lab-0.2.1/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.0/quant_invest_lab/simulation.py` & `quant_invest_lab-0.2.1/quant_invest_lab/simulation.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.0/quant_invest_lab/utils.py` & `quant_invest_lab-0.2.1/quant_invest_lab/utils.py`

 * *Files identical despite different names*

